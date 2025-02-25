# Global-Water-Access-Analysis

A data analysis project examining global access to drinking water using country-level statistics. Based on WHO/UNICEF Joint Monitoring Programme (JMP) data.

![Water Access Visualization Concept](https://via.placeholder.com/800x400.png?text=Water+Access+Visualization)

## Dataset Overview
**File:** `Global Drinking Water Access.xlsx`

### Sheets:
1. **Estimates-on-the-use-of-water-(**
   - Contains country-level data for 214 regions
   - Key metrics:
     - Population statistics (urban/rural)
     - Water access types: 
       - Basic services (`wat_bas`)
       - Limited services (`wat_lim`)
       - Unimproved sources (`wat_unimp`)
       - Surface water (`wat_sur`)
     - Income group classifications

2. **Global 2020 report**
   - Aggregated statistics with formulas calculating:
     - Global population coverage
     - Water access metrics (max, min, mean, median)
     - Comparative analysis between urban/rural populations
     - Statistical measures (standard deviation, quartiles)

3. **Visuals/Pivot Tables**
    - National population vs Urban and rural share
    - National distribution of access to water per service level
    - Urban distribution of access per service level
    - Rural distribution of access per service level

## Key Metrics
- Total global population without safe water: **2.2 billion**
- Urban populations with basic water access: **97.6% (max)** vs **37.2% (min)**
- Rural populations using surface water: **40.5% (max)**
- Income group correlation:
  - High-income countries: **99.9%** basic access
  - Low-income countries: **46.9%** basic access

## Usage
1. **Data Exploration**:
   ```excel
   =SUM('Estimates-on-the-use-of-water-('!E2:E214)*1000  // Total population calculation
   =AVERAGE('Estimates-on-the-use-of-water-('!K2:K214)   // Average basic water access
