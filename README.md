# realestateanalyzer
Real Estate Analyzer courtesy of CC/Gemini :)

# 🏠 Real Estate Investment Analyzer Pro

A powerful, professional-grade real estate investment analysis tool for buy-and-hold investors. Analyze properties across multiple markets with comprehensive metrics, stress testing, and 10-year projections—all in a single HTML file with no installation required.

## ✨ Features

### 📊 **Comprehensive Analysis Dashboard**
- **Sortable Property Table** - Click any column header to sort properties by address, market, price, bedrooms/bathrooms, rent, cash flow, CoC%, cap rate, or DSCR
- **Property Overview** - See key property details including beds/baths at a glance
- **Summary Statistics** - Track total properties, passing investments, average CoC return, and total monthly cash flow
- **Real-time Search** - Filter properties instantly by address
- **Pass/Fail Indicators** - Visual status showing which properties meet your investment criteria

### 💰 **Investment Metrics**
- **Cash-on-Cash Return** - Annual cash flow as % of total cash invested (8% minimum hurdle rate)
- **Cap Rate** - Net Operating Income as % of purchase price (6% minimum hurdle rate)
- **DSCR (Debt Service Coverage Ratio)** - NOI divided by annual debt service (1.25 minimum hurdle rate)
- **Monthly & Annual Cash Flow** - Complete income and expense projections
- **NOI (Net Operating Income)** - Professional-grade income/expense calculations

### 🔬 **Stress Testing**
Three conservative scenarios to test property resilience:
- **25% Vacancy Spike** - Tests ability to handle extended vacancies
- **17.5% Expense Surge** - Models unexpected cost increases
- **12.5% Rent Decrease** - Evaluates downside risk from market softening

Each test shows resulting NOI, cash flow (annual/monthly), and pass/fail status.

### 📈 **10-Year Wealth Building Projections**
- **Detailed Year-by-Year Breakdown** - Rental income, expenses, NOI, cash flow, principal paydown, remaining loan balance, property value, and equity
- **Cash Flow Chart** - Visual representation of annual and cumulative cash flow over time
- **Equity Build-Up Chart** - Stacked bar chart showing loan balance vs equity growth
- **Compound Growth Modeling** - Rent growth and expense growth applied year over year

### 🗺️ **Custom Market Management** *(v4 Feature)*
- **Add Unlimited Markets** - Define your own markets beyond Tampa and Atlanta defaults
- **Custom Parameters** - Set property tax rate, insurance costs, vacancy rate, appreciation, and rent growth for each market
- **Edit & Delete** - Full CRUD operations on custom markets (defaults are protected)
- **Persistent Storage** - Markets saved to localStorage for future sessions
- **Smart CSV Matching** - Auto-assigns properties to markets based on city names during CSV import

### 📋 **Comparable Properties**
- **Manual Entry** - Add comparable properties with address, sqft, beds/baths, rent, and sale price
- **CSV Import** - Bulk import comps from MLS data
- **$/SqFt Analysis** - Automatic price per square foot calculations
- **Instant Equity Estimation** - Compare purchase price to market value based on comps

### 💾 **Data Management**
- **Auto-Save** - Properties automatically saved to browser localStorage
- **Export to JSON** - Download all property data for backup or sharing
- **Import from JSON** - Restore previous sessions or share property portfolios
- **CSV Import** - Import properties from MLS exports (auto-detects Tampa/Atlanta/custom markets)
- **Comparable CSV Import** - Bulk import comparable property data

### ⚙️ **Global Settings Sidebar**
- **Market Selection** - Choose from Tampa, FL, Atlanta, GA, or your custom markets
- **Financing Controls** - Adjust down payment %, interest rate, and loan term globally
- **Operating Expense Assumptions** - Set vacancy rate, property management %, maintenance reserve %, and CapEx reserve %
- **Growth Assumptions** - Configure appreciation rate, rent growth, and expense growth rates

### 🎨 **Modern Professional UI**
- **Dark Sidebar Navigation** - Clean, organized control panel
- **Card-Based Layouts** - Professional metric displays with color-coded indicators
- **Sticky Table Headers** - Maintain context while scrolling through property lists
- **Responsive Design** - Works on desktop, tablet, and mobile devices
- **Color-Coded Metrics** - Green for passing, red for failing investment thresholds

## 🚀 Getting Started

### Installation

**No installation required!** This is a single-file HTML application.

1. Download `real-estate-analyzer-v4.html`
2. Open it in any modern web browser (Chrome, Firefox, Safari, Edge)
3. Start analyzing properties immediately

That's it! No servers, no dependencies, no setup.

### Quick Start

1. **Select Your Market** - Choose Tampa, Atlanta, or add your own custom market
2. **Set Global Assumptions** - Configure financing terms and expense ratios in the sidebar
3. **Add a Property** - Click "+ Add Property" and enter property details
4. **View Analysis** - Instantly see metrics, stress tests, and projections
5. **Save Your Work** - Properties are automatically saved to your browser

## 📖 How to Use

### Adding Your First Property

1. Click **"+ Add Property"** in the sidebar (or use the Add/Edit tab)
2. Fill in basic information:
   - Address
   - Purchase price
   - Square footage, bedrooms, bathrooms
   - Year built
3. (Optional) Override market defaults:
   - Monthly rent (defaults to 1% of purchase price)
   - Property tax and insurance
   - HOA fees and utilities
4. (Optional) Add comparable properties for market value estimation
5. Click **"Save Property"**

### Analyzing Properties

**Dashboard View:**
- See all properties in a sortable table with key details (address, market, price, beds/baths, rent, cash flow, metrics)
- Click column headers to sort by any metric including bedrooms/bathrooms
- Use the search bar to filter by address
- Click "View" to see detailed analysis

**Detailed Analysis Tab:**
- 4 key metrics at the top (Monthly CF, CoC%, Cap Rate, DSCR)
- Pass/Fail alert banner for hurdle rates
- Complete income statement breakdown
- Operating expenses detail
- Financing and cash flow summary
- Comparable properties (if added)

**Stress & Projections Tab:**
- 3 stress test scenarios with pass/fail indicators
- 10-year detailed projection table
- Cash flow over time chart
- Equity build-up over time chart

### Managing Markets (v4)

1. Click **"⚙️ Manage Markets"** in the sidebar
2. View existing markets (default and custom)
3. To add a new market:
   - Enter market name (e.g., "Phoenix, AZ")
   - Set property tax rate (%)
   - Enter annual insurance cost
   - Set vacancy rate, appreciation, and rent growth
   - Click "Add Market"
4. Edit or delete custom markets using the buttons (defaults are protected)

### Importing Data

**CSV Import (Properties):**
- Click "Import CSV" in the sidebar
- Select a CSV file with columns: Address, City, Price, Square Footage, Beds, Baths
- Properties will be auto-assigned to matching markets
- Review and analyze imported properties

**CSV Import (Comparables):**
- From the Add/Edit tab, click "Import CSV" under Comparable Properties
- Select a CSV with comparable property data
- Automatically populates comp fields for analysis

## 📊 Default Markets

### Tampa, FL
- Property Tax: 0.9%
- Insurance: $2,500/year
- Vacancy Rate: 8%
- Appreciation: 2.5%/year
- Rent Growth: 3.0%/year

### Atlanta, GA
- Property Tax: 1.0%
- Insurance: $1,500/year
- Vacancy Rate: 9%
- Appreciation: 3.0%/year
- Rent Growth: 3.5%/year

## 🎯 Investment Hurdle Rates

Properties are evaluated against these minimum thresholds:

- **Cash-on-Cash Return:** ≥ 8%
- **Cap Rate:** ≥ 6%
- **DSCR:** ≥ 1.25

Properties passing all three hurdles are marked with ✓ in green.

## 🧮 Calculation Methodology

### Cash Flow Formula
```
Gross Rent + Other Income
- Vacancy Loss (% of gross income)
= Effective Gross Income

- Property Tax
- Insurance
- HOA Fees
- Property Management (% of gross rent)
- Maintenance Reserve (% of gross rent)
- CapEx Reserve (% of gross rent)
- Utilities
= Net Operating Income (NOI)

- Annual Debt Service (P&I payments)
= Annual Cash Flow
```

### Key Metrics
- **Cash-on-Cash Return** = (Annual Cash Flow / Total Cash Invested) × 100
- **Cap Rate** = (NOI / Purchase Price) × 100
- **DSCR** = NOI / Annual Debt Service

### 10-Year Projections
- Rent increases by growth rate % each year
- Fixed expenses (tax, insurance) grow by expense growth rate
- Variable expenses (mgmt, maint, capex) calculated as % of current rent
- Property value compounds by appreciation rate
- Principal paydown calculated monthly with accurate amortization
- Equity = Property Value - Remaining Loan Balance

## 🔧 Technical Details

### Built With
- **Vanilla JavaScript** - No frameworks, pure ES6+
- **Chart.js** - For cash flow and equity visualizations (CDN)
- **localStorage API** - For persistent data storage
- **CSS Grid & Flexbox** - Modern responsive layouts

### Browser Compatibility
- Chrome/Edge (recommended)
- Firefox
- Safari
- Any modern browser with ES6 support and localStorage

### File Size
- Single HTML file (~70KB)
- No external dependencies except Chart.js CDN
- All CSS and JavaScript inline for portability

### Data Storage
- **Properties:** localStorage key `savedProperties`
- **Custom Markets:** localStorage key `customMarkets`
- Data persists until browser cache is cleared
- Export to JSON for permanent backup

## 📝 Version History

### v4 - Custom Market Management & Enhanced Dashboard
- ✨ Add unlimited custom markets with configurable parameters
- ✨ Edit and delete custom markets
- ✨ Smart CSV import with market matching
- ✨ Protected default markets (Tampa, Atlanta)
- 🔄 Dynamic market selector that scales with added markets
- 📊 Beds/Baths column added to dashboard for quick property overview

### v3 - Modern UI & Sortable Dashboard
- 🎨 Professional dark sidebar design
- 📊 Sortable columns in property dashboard
- 📈 Summary statistics cards
- 🔍 Real-time property search
- 💾 Improved data persistence

### v2 - Enhanced Analytics
- 🔬 3-scenario stress testing
- 📈 10-year projections with charts
- 📋 Comparable properties analysis
- ⚙️ Global settings sidebar

### v1 - Initial Release
- 💰 Core investment metrics (CoC, Cap Rate, DSCR)
- 🏘️ Tampa & Atlanta market presets
- 💾 Save/load functionality

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:

- **Report Bugs** - Open an issue describing the problem
- **Suggest Features** - Share ideas for new functionality
- **Submit Pull Requests** - Fork, make changes, and submit PR
- **Share Feedback** - Let us know how you're using the tool

### Feature Ideas
- [ ] Multi-property portfolio summaries
- [ ] PDF export for reports
- [ ] Loan comparison calculator
- [ ] Property tax appeal tracker
- [ ] Rental income tracking
- [ ] Expense tracking and reconciliation

## 📄 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2025

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## ⚠️ Disclaimer

This tool is for educational and informational purposes only. It is not financial, investment, or legal advice. Always:

- Conduct thorough due diligence on any investment property
- Consult with qualified professionals (CPAs, real estate attorneys, etc.)
- Verify all assumptions and calculations independently
- Consider your individual financial situation and risk tolerance
- Understand that past performance does not guarantee future results

Real estate investing involves significant risk. Use this tool as one component of your research process, not as the sole basis for investment decisions.

## 🙏 Acknowledgments

- Built with vanilla JavaScript for maximum portability
- Chart.js for beautiful data visualizations
- Inspired by real buy-and-hold investors analyzing properties across markets

## 📬 Support

Questions? Issues? Suggestions?

- **Open an Issue** - Use GitHub Issues for bug reports and feature requests
- **Discussions** - Share your success stories and ask questions

---

**Made with ❤️ for real estate investors**

*Analyze smarter. Invest better.*
