# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-file HTML application called "NBFC Quant Toolbox" - a comprehensive suite of 70+ financial tools for Non-Banking Financial Companies (NBFCs). The entire application runs 100% client-side in the browser with no server component.

## Architecture

**Single Monolith File**: `hundredapps.html` (~178KB, ~4600 lines)
- Self-contained HTML/CSS/JavaScript application
- All tool logic is inline JavaScript within a single `<script>` tag
- Uses Tailwind CSS via CDN for styling

**External Libraries** (loaded via CDN):
- PapaParse: CSV parsing
- Plotly.js: Interactive charts
- Chart.js: Additional charting
- docx: Word document generation
- jStat: Statistical functions (normal distribution, etc.)

**Core Structure**:
1. `TOOL_METADATA` array (line ~113): Main tools with full implementations
2. `PROTOTYPE_APPS` array (line ~158): Placeholder/prototype tools
3. `ALL_TOOLS`: Combined array for the tool selector
4. Tool renderer functions: `render<ToolName>()` pattern (e.g., `renderSecuritisationSuite()`)

**Application Flow**:
- Tool selector dropdown populated from `ALL_TOOLS`
- `renderToolBody()` maps tool type to renderer function
- Each tool has metadata: id, title, shortDescription, type, inputColumns, usageNotes

## Key Tool Categories

- **Securitisation Suite**: PTC waterfall modeling, Gaussian Copula LE, CE calculation
- **Lending Calculators**: FOIR, LAP, education loans, SCF discounting
- **Risk Tools**: NPA provisioning (IRAC), static pool analysis, roll-rate matrices
- **Treasury**: XIRR, HPR, ALM stress testing, duration analysis
- **Collections**: PTP tracker, settlement optimizer, cure rate forecasting

## Development Notes

- Financial calculations use helper functions: `calcEmi()`, `loanFromEmi()`, `normCdf()`, `normInv()`
- Date handling: `formatDateFlexible()` handles multiple date formats
- Currency formatting: `moneyFmt` (INR), `pct()` for percentages
- CSV export: `downloadCSV()` utility function
- No build process - edit HTML directly and refresh browser to test
