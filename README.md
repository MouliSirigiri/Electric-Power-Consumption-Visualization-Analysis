#**Electric Power Consumption Visualization Analysis**

#**Overview**

This repository contains Python code for exploratory data analysis and visualization of electric power consumption (kWh per capita) across 8 countries: Australia, Canada, China, India, Russia, United Arab Emirates (UAE), United Kingdom (UK), and United States (USA). The analysis uses data from 2001–2014 to create time-series line plots, a bar chart for a specific year (2008), and pie charts for relative comparisons in 2001 and 2014. Built with Pandas and Matplotlib, it highlights trends like China's rapid growth and Canada's consistent high consumption.

**Key goals:**

Track temporal changes in per-capita electricity use.
Rank countries by consumption in a snapshot year.
Compare relative shares over a decade to spot shifts.

Insights: China's consumption tripled (from ~1,200 to 3,600 kWh/capita), while India remained the lowest; Canada topped rankings throughout.

#**Key Findings**

Trends (Line Plot): Stable consumption in most countries; China +200% growth; Canada >15,000 kWh/capita consistently; India <1,000.
2008 Ranking (Bar Chart): Canada (16,377.5) > USA (12,991) > UAE (13,500? – data-specific); Russia/UK ~6,500–6,800; India ~600.
Relative Shares (Pie Charts): 2001: USA/Canada ~25–28%; 2014: China rises to 23%, others dip slightly.

#**Summary Table (kWh per Capita, Approx.)**

Country,2001,2008,2014,% Change
Australia,"10,257","10,800","10,550",+3%
Canada,"16,800","16,377","15,600",-7%
China,"1,200","2,800","3,600",+200%
India,500,600,800,+60%
Russia,"6,500","6,800","7,000",+8%
UAE,"12,000","13,500","11,500",-4%
UK,"6,200","6,400","5,900",-5%
USA,"12,500","12,991","12,900",+3%

#**Data Sources**

Primary: World Bank via Google Drive CSV.
Years: 2001–2014; 8 countries.
Indicator: Electric power consumption (kWh per capita).

#**Methods**

Preprocessing: Pandas for cleaning (dropna, rename).
Plots:
Line: plt.plot() with labels/legend.
Bar: plt.bar() with value labels via custom function.
Pie: plt.pie() with % autopct, adjusted distances.

Figure Sizing: Consistent (10x8 for line, 16x6 for bar, 8x5 for pies).

#**Limitations and Future Work**

Static years; extend to 2020+ with updated data.
No stats (e.g., correlations); add regression for forecasts.
Enhance: Interactive plots with Plotly; include GDP correlations.
