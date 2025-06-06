# ⚡ Generator Bidding Behaviour Analysis (NEM 2025)

This project analyzes the bidding behavior of electricity generators in the Australian National Electricity Market (NEM) in 2025, focusing on how different generation types—Solar, OCGT (gas), and Black Coal—strategically submit bids under varying price and time conditions.

---

##  Objective

To understand how generator bidding strategies reflect their operational characteristics, market roles, and response to price signals—particularly:
- Distribution of bids across price bands
- Hourly bid price trends
- Aggregated supply curves
- Differences in peak vs off-peak behavior

---

##  Tools & Libraries

- Python (Pandas, Seaborn, Matplotlib)
- Jupyter Notebook
- CSV Bidding Data from NEM
- Power BI (optional for dashboard version)

---

##  Key Analyses

### 1.  Bid Distribution by Price Bin

- **Solar** bids are almost entirely in the `<= 0` range, confirming their need for constant dispatch and zero marginal cost.
- **Black Coal** shows a diversified strategy across low, medium, and high prices.
- **OCGT** bids only in the `301–1000` range, matching their role as expensive peaker plants.

*Insight:* Generator type directly determines price band positioning.

---

### 2.  Hourly Bid Price Trends

Line plot of average bid price by hour of day reveals:

- **Solar:** Flat, low bids between 8 AM – 6 PM (daylight hours)
- **Black Coal:** Moderate prices (~$4800–5600/MWh) with minor peaks at 4 AM and 4–6 PM
- **OCGT:** Highest bids (~$16,000–17,000/MWh) spiking around peak demand hours

 *Insight:* Generators bid to align with their cost structures and expected dispatch windows.

---

### 3.  Aggregated Supply Curves

- **Solar and Coal** show smoother cumulative supply curves, indicating broader volume availability.
- **OCGT** has a steep, sudden curve — tiny volumes at very high prices.

*Insight:* Supply shape reflects flexibility vs scarcity. OCGT is scarce but expensive.

---

### 4.  Peak vs Off-Peak Analysis

- Defined Peak: 6–10 AM & 4–9 PM
- Solar bids are unaffected by time (sunlight-based).
- OCGT raises prices during peak hours.
- Black Coal offers largest volume consistently but increases MW during peak.

*Insight:* Bidding strategies adapt to demand cycles and generator roles.

---

## 📁 Outputs

| Output                              | Description                                              |
|-------------------------------------|----------------------------------------------------------|
| `price_bin_bar.png`                | Volume vs price bin by generation type                  |
| `hourly_avg_price_lineplot.png`    | Hourly price trend by technology                        |
| `supply_curve.png`                 | Aggregated supply curves by generator                   |
| `peak_offpeak_barplots.png`        | Avg bid price and MW offered (Peak vs Off-Peak)         |

---

## 📬 Authors

**Ananya Pandey**  
*Master of Business Analytics, Macquarie University*  
📧 Email: [pandey.ananya472@gmail.com]  
🔗 LinkedIn: [[linkedin.com/in/ananyapandey](https://www.linkedin.com/in/ananyapandey99/)](#)

---

##  Summary

This analysis provides a deep dive into how Solar, Coal, and OCGT generators differ in pricing strategy and bidding behavior. The insights can support market operators, regulators, and analysts in understanding dispatch logic and market efficiency under evolving energy mixes.

