# Levelized-Cost-of-Electricity-LCOE-Prediction-Project
Machine learning project focused on predicting the Levelized Cost of Electricity (LCOE) for utility-scale solar PV using multi-country renewable energy datasets.

### Dataset Description

The dataset used in this study is compiled from international renewable energy cost and deployment sources and contains country-level observations of utility-scale solar photovoltaic (PV) projects. The dataset combines technical, economic, and regional information to support the modelling of the Levelized Cost of Electricity (LCOE). The final dataset includes 2,396 observations, of which 2,011 correspond to utility-scale Solar PV, spanning multiple countries, regions, and years.


| Variable Name | Unit | Description | Used in ML Model |
| :--- | :--- | :--- | :--- |
| **LCOE** | $/kWh | Levelized Cost of Electricity: average cost of generating one kilowatt-hour over the project lifetime | **Target** |
| **Total installed costs** | $/kW | Total upfront investment cost, including modules, balance-of-system, and installation | (if available) |
| **Module costs** | $/kW | Cost of solar PV modules per kilowatt | |
| **Balance of Systems Cost** | $/kW | Cost of non-module components such as inverters, mounting, wiring, and labour | (used only to reconstruct total cost) |
| **Capacity** | MW | Installed capacity of utility-scale solar PV projects | |
| **Production / CF** | GWh / fraction | Electricity generated / Ratio of actual electricity generation to maximum possible generation | (fixed or cleaned) |
| **WACC** | % (decimal) | Weighted Average Cost of Capital reflecting financing conditions | |
| **CRF / year** | year | Financial factor derived from WACC and project lifetime / Year of project commissioning | (contextual feature) |
| **Country** | - | Country associated with each observation | |
| **Country Code** | - | ISO country code | |
| **Region** | - | Geographic grouping of countries (e.g., Europe, MENA, Asia) | |
| **IncomeGroup** | - | Country income classification | (optional) |
| **BidYield** | - | Auction bid-related metric | X |
| **TECHNOLOGY RISK** | - | Technology-specific risk indicator | X |
