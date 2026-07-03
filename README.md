# El Paso First-Time Homebuyer Analysis

A comprehensive, data-driven analysis and interactive dashboard examining first-time homebuyer patterns, affordability, mortgage strategies, and policy recommendations for El Paso, Texas.

**Live Demo:** [[View Site](https://hoffmanap.github.io/el-paso-homebuyer/)]

## Project Overview

This analysis examines 849 first-time homebuyer transactions in El Paso County (2025), revealing insights into:
- Demographic profiles (age, income, origin)
- Geographic concentration patterns
- Affordability and price-to-income analysis
- Mortgage product strategies (FHA, VA, conventional)
- Data-backed policy recommendations for housing supply and affordability

## Files Included

```
your-repo/
├── index.html              # Landing page & overview
├── analysis.html           # Full demographic & geographic analysis with charts
├── mortgage.html           # Deep-dive into mortgage product strategy
├── map.html                # Interactive Leaflet map of zip code concentration
├── policy.html             # Data-backed policy recommendations
├── data.csv                # Extracted data for reference
└── README.md               # This file
```

## Quick Start: Deploy to GitHub Pages

### Step 1: Create Repository
```bash
# Create new repo on GitHub
# Name: `el-paso-homebuyer` (or your preferred name)
# Make it PUBLIC
# Do NOT initialize with README (you'll add these files instead)

# Clone locally
git clone https://github.com/YOUR-USERNAME/el-paso-homebuyer.git
cd el-paso-homebuyer
```

### Step 2: Add Files
Copy all HTML files and the CSV file into your repository root:
```
index.html
analysis.html
mortgage.html
map.html
policy.html
data.csv
README.md
```

### Step 3: Commit & Push
```bash
git add .
git commit -m "Initial commit: El Paso homebuyer analysis dashboard"
git push origin main
```

### Step 4: Enable GitHub Pages
1. Go to your repo **Settings** → **Pages**
2. Under "Source," select **main** branch
3. Click **Save**
4. Your site will be live at: `https://YOUR-USERNAME.github.io/el-paso-homebuyer/`

**That's it!** Your site is now live.

---

## Site Structure

### `index.html` - Landing Page
Overview of the analysis with key metrics, buyer demographics, origin patterns, affordability analysis, and calls-to-action to other pages.

- **Audience:** Decision-makers, policymakers, developers, general public
- **Key sections:** Market overview, buyer demographics, origin patterns, affordability, housing product, mortgage overview

### `analysis.html` - Full Analysis
Comprehensive demographic breakdowns with interactive Plotly charts showing age, income, origin, destinations, housing product, and mortgage products.

- **Audience:** Policy analysts, planners, researchers
- **Key visualizations:** Age/income distributions, pie charts for origin, bar charts for destination zip codes, mortgage product mix

### `mortgage.html` - Mortgage Strategy
Deep-dive into FHA, VA, and conventional lending products with program comparisons, cost/benefit analysis, and policy implications.

- **Audience:** Lenders, policy makers, real estate professionals
- **Key sections:** FHA entry-point dominance, VA military advantage, conventional upper-tier concentration, program comparisons

### `map.html` - Interactive Map
Leaflet.js map showing zip code boundaries, buyer concentration, and pop-up data for each area. Sidebar displays top-3 concentrated areas.

- **Audience:** Real estate developers, planners, investors
- **Key feature:** Click zip codes to see purchase counts and percentages

### `policy.html` - Policy Recommendations
Data-backed strategies for zoning, building code, and incentive programs tied to specific metrics from the analysis.

- **Audience:** City planners, elected officials, housing advocates
- **Key sections:**
  - Zoning reforms (upzoning, ADUs, parking reduction)
  - Building code streamlining (performance-based review, expedited permitting)
  - Down-payment assistance programs
  - Implementation timeline and funding

---

## Data Source & Methodology

**Sample:** 849 first-time homebuyer transactions (2025)
- **Definition:** Primary home purchase loans, borrowers aged 25–44
- **Loan types:** FHA, VA, conventional, USDA

**Data sources:**
- **HMDA** (Home Mortgage Disclosure Act): Loan terms, demographics, underwriting outcomes
- **MLS** (Multiple Listing Service): Property characteristics, pricing, location
- **Data Axle:** Historical mover tracking, prior geographic locations

**Geographic scope:** El Paso County, Texas (zip codes, origin states, destination areas)

---

## Key Findings

| Metric | Value |
|--------|-------|
| **Total Buyers Analyzed** | 849 |
| **Median Purchase Price** | $267,000 |
| **Median Household Income** | $97,000 |
| **Price-to-Income Ratio** | 2.75x |
| **Top Destination (79928)** | 27.0% of purchases |
| **Texas-origin Buyers** | 73.9% |
| **FHA Loans** | 43.6% |
| **VA Loans** | 33.7% |
| **Govt-Backed Lending** | 77.3% |

---

## Policy Recommendations Summary

### I. Zoning & Land Use
- Upzone secondary corridors (79912, 79936) for mixed-use/multifamily
- Legalize accessory dwelling units (ADUs)
- Reduce parking minimums by 50%
- Create opportunity zones with fee waivers

### II. Building Code
- Adopt performance-based code for affordable housing
- Standardize utility infrastructure
- Expedited permitting (60-day timeline)

### III. Down-Payment & Financing
- City-funded down-payment assistance ($2M annually, $10k per household)
- Community land trust (CLT) pilot (50 units over 3 years)
- Shared equity purchase program
- Employer-matched down-payment incentives

### IV. Expected Outcomes (Year 3)
- 250–300 new units in opportunity zones
- 280 households assisted via down-payment programs
- 30–50 CLT homes closed
- Maintained affordability (2.75x P/I) for local buyers

---

## Navigation & User Experience

**Top Navigation Bar** (fixed, all pages):
- Logo → links to index.html
- Links: Overview | Full Analysis | Mortgage Strategy | Geographic Map | Policy

**Color Scheme:**
- Primary blue: `#2d5a7b` (headers, key data)
- Accent orange: `#e07856` (highlights, call-to-action)
- Neutral grays: `#64748b`, `#475569` (body text)
- Light backgrounds: `#fafbfc`, `#f8f9fa`

**Responsive Design:**
- Desktop: Full layout with sidebars
- Tablet: Single-column layout
- Mobile: Stacked sections, hidden navigation

---

## Technology Stack

- **HTML5** / **CSS3** / **Vanilla JavaScript** (no framework dependencies)
- **Plotly.js** - Interactive data visualizations
- **Leaflet.js** - Interactive mapping
- **Google Fonts** (Inter typeface)
- **CDN-hosted libraries** (no build process required)

## Customization

### Change Title/Branding
Edit the `<title>` tag in each HTML file, and update the `nav .logo` text.

### Update Data
Edit `data.csv` with new metrics, or update chart data directly in JavaScript at the bottom of each page.

### Modify Colors
Search for color hex codes in `<style>` blocks:
- `#2d5a7b` → primary blue
- `#e07856` → accent orange
- Replace globally to rebrand

### Add New Pages
Create a new `.html` file, copy the navigation bar from `index.html`, and link it in the `nav .links` section.

---

## Performance Notes

- All resources load from CDN (Plotly, Leaflet, Google Fonts)
- No server-side processing required
- Site works entirely in-browser
- Responsive to 640px+ (mobile-optimized)

---

## License & Attribution

Data is based on HMDA, MLS, and Data Axle sources. Analysis and visualizations are original work.

For questions or improvements, create an issue or pull request in this repository.

---

## Next Steps

1. **Deploy:** Follow "Quick Start" above
2. **Customize:** Update colors, branding, contact info as needed
3. **Share:** Link to your live site in planning documents, presentations, social media
4. **Iterate:** Update data and analysis annually to track trends

---

**Questions?** Refer to the individual page sections above or review the HTML files directly—all code is documented and readable.

**Last updated:** July 2025
