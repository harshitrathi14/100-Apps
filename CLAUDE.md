# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Single-file HTML application "NBFC Quant Toolbox" - a suite of 200+ financial tools for Non-Banking Financial Companies (NBFCs) and banks. Runs 100% client-side with IndexedDB/LocalStorage persistence.

## Architecture

**Single File**: `thousandapps.html` (~7200 lines, ~280KB)

**External Libraries** (CDN):
- PapaParse: CSV parsing
- Plotly.js + Chart.js: Charting
- docx: Word document generation
- jStat: Statistical functions (normal distribution, etc.)
- Tailwind CSS: Styling

**Core Structure**:
```
Lines 1-86:     HTML + CSS (navigation, tool cards, save toolbar)
Lines 199-350:  NBFCStorage module (IndexedDB persistence layer)
Lines 350-600:  TOOL_METADATA array (200+ tool definitions)
Lines 600-750:  Core app logic (renderToolBody, navigation, search)
Lines 750-7200: Render functions for each tool
```

**Persistence Layer** (`NBFCStorage`):
- `Preferences`: LocalStorage for theme, favorites, recent tools
- `ToolState`: IndexedDB for saved tool inputs (per-tool, named slots)
- `Datasets`: IndexedDB for large CSV data
- `Backup`: Export/import all data as JSON

**Tool Categories** (15 departments):
Retail Lending, MSME & Corporate, Collections & Recovery, Risk & Compliance, Treasury & ALM, Securitisation, Operations, Pricing & Profitability, Regulatory, Microfinance, Cards & Digital, MIS & Reporting, Data Quality & Utilities, Underwriting & Policy

## Adding New Tools

1. Add entry to `TOOL_METADATA` array:
```javascript
{
  id: 'toolId',
  title: 'Tool Title',
  shortDescription: 'One line description.',
  usageNotes: ['Usage instruction 1', 'Usage instruction 2'],
  type: 'toolId',  // matches render function name
  category: 'Retail Lending',
  inputColumns: [{ name: 'col', description: 'Desc', required: true }]
}
```

2. Add render function following this pattern:
```javascript
function renderToolId() {
  const c = document.getElementById('tool-container');
  c.innerHTML = `
    ${renderSaveToolbar('toolId')}
    <div class="max-w-2xl mx-auto bg-white border rounded-xl shadow p-6">
      <h3 class="text-lg font-bold text-slate-800 mb-4">Tool Title</h3>
      <div class="grid grid-cols-2 gap-4 mb-4">
        <div>
          <label class="block text-xs font-medium text-slate-600 mb-1">Input Label</label>
          <input id="toolId-input1" type="number" class="w-full border rounded px-3 py-2" value="0">
        </div>
      </div>
      <button onclick="window.calcToolId()" class="w-full bg-indigo-600 text-white py-2 rounded-lg font-semibold hover:bg-indigo-700">Calculate</button>
      <div id="toolId-result" class="mt-4"></div>
    </div>`;
}
window.calcToolId = function() {
  const input1 = parseFloat(document.getElementById('toolId-input1').value) || 0;
  // Calculate result
  document.getElementById('toolId-result').innerHTML = `<div class="bg-green-50 border border-green-200 rounded-lg p-4">Result: ${result}</div>`;
  saveToolState('toolId');
};
```

3. Add case in `renderToolBody()` switch statement if using custom type.

## Key Helper Functions

- `calcEmi(p, r, n)`: EMI calculation (reducing balance)
- `loanFromEmi(emi, r, n)`: Reverse EMI to principal
- `normCdf(z)`, `normInv(p)`: Normal distribution functions
- `formatDateFlexible(d)`: Parse multiple date formats
- `moneyFmt(n)`: Format as INR (₹1,23,456)
- `pct(n, d)`: Format as percentage
- `downloadCSV(data, filename)`: Export data as CSV
- `renderSaveToolbar(toolId)`: Reusable save/load toolbar HTML
- `saveToolState(toolId)`: Persist current inputs to IndexedDB

## Development

No build process - edit HTML directly and refresh browser to test.
