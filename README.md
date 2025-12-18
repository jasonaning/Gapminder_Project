# EXPLORING GLOBAL ECONOMIC DEVELOPMENT TRENDS (1952 - 2007) USING GAPMINDER
---

## Table of Contents  
1. [Project Overview](#project-overview)  
2. [Objectives](#objectives)  
3. [Dataset Description](#dataset-description)   
4. [Key Insights](#key-insights)  
5. [Technologies Used](#technologies-used)  
6. [Results](#results)
7. [Conclusion](#conclusion)  
 ---

12. ## PROJECT OVERVIEW
Development economics focuses on understanding why some countries live longer, earn higher incomes, and grow faster than others. The Gapminder dataset provides a clear picture of how life expectancy, income levels, population, and economic growth have changed across the world from 1952 to 2007.
This study was done to:
- Compare the development performance of countries and continents.

- Understand how income influences life expectancy.

- Identify which countries are growing fast and which ones are lagging behind.

- Reveal long-term global inequality patterns in health and income.
  
  ---

 ## OBJECTIVES
 The Gapminder data helps policymakers, investors, and development agencies understand how income growth, population change, and health    outcomes interact globally, enabling smarter economic and social decisions.
 
---

1. **Understand how income affects health outcomes**:
 Measure how GDP per capita influences life expectancy across countries and over time.
 Help governments justify economic growth as a health investment.

2. **Track economic progress over time**:
Measure global GDP growth from 1952 to 2007. Identify countries with the fastest long-run GDP growth. Useful for long-term investment and development planning.

3. **Identify income inequality across continents**:
Compare GDP distribution by continent using boxplots. Support targeted development funding for low-income regions (especially Africa).

4. **Rank countries by demographic and economic importance**:
Identify countries with the largest average populations. Useful for market sizing, public service delivery, and global business strategy.

---

## DATASET DESCRIPTION 
- The dataset used in this analysis is the Gapminder dataset, a widely used panel dataset in development economics and social science research. Gapminder contains country-level data observed over time (1952–2007, every 5 years) and is designed to study long-run relationships between economic growth, population dynamics, and human development.

**Structure of the Dataset**
- Type: Panel (longitudinal) data
- Observations: 1,704 country–year observations
- Countries: 142
- Time period: 1952 to 2007 (5-year intervals)
  
**The dataset used in the Gapminder contains the following columns:** 

| Column       | Description                            |  
|--------------|----------------------------------------|  
| Country      | Country name                           |  
| Continent    | Continent classification               |  
| Year         | Observation year                       |  
| Pop          | Total population                       |  
| gdpPercap    | Gross Domestic Product per capita (USD)|  
| lifeExp      | Life expectancy at birth (years)       |  

---

## KEY INSIGHTS  
- **Income is the strongest global predictor of health:**
Across countries and over time, higher GDP per capita consistently leads to significantly higher life expectancy, with fixed-effects models confirming this relationship within countries.

- **Diminishing returns to income are evident:**
Life expectancy rises rapidly at low income levels but increases much more slowly beyond middle-income thresholds, indicating that growth alone cannot indefinitely improve health outcomes.

- **Population size has weak explanatory power for health:**
Despite vast differences in population, the correlation between population and life expectancy is low, showing that how rich a country is matters more than how large it is.

- **Global inequality remains structurally high:**
The Gini coefficient (~0.55) and Lorenz curve reveal persistent long-run income concentration, where a small group of countries capture a disproportionate share of global income.

- **Economic growth is volatile and uneven across regions:**
GDP growth rates and volatility differ sharply by continent, with developing regions experiencing higher instability, posing challenges for sustained development and long-term planning.

---

## Technologies Used  

- **Programming Language**: Rstudios  
- **Packages**: tidyverse, gapminder, plm, lme4, tseries, psych, ineq, forecast, lmtest 
- **Tools**:  R Jupyter Notebook, Github, Latex(Mathematical Formulars)  

---

## Results & Discussion 

Panel and regression analysis confirm GDP significantly increases life expectancy (FE p < 0.01, Hausman test favors FE); t-tests and ANOVA show income growth 1952–2007 is significant, while Breusch-Pagan, Shapiro, and correlation tests highlight variance heterogeneity and weak population-life links. Time series (ADF, ARIMA), clustering (k = 3), and inequality metrics (Gini ≈ 0.55, CV = 1.2) reveal volatility, distributional disparities, and persistent global inequality.

---

## Conclusion & Recommendation
Empirical evidence shows a strong positive correlation between GDP per capita and life expectancy *(r ≈ 0.85, p < 0.01)*, while population growth exhibits only a weak link (r ≈ 0.12). Panel data and FE models confirm income significantly drives health improvements within countries, with diminishing returns beyond middle-income levels. Inequality remains high globally (Gini ≈ 0.55, P90/P10 ≈ 12), highlighting persistent disparities in wealth and well-being. Policy interventions should focus on targeted health and education investments alongside inclusive economic growth to reduce inequality. Sustained GDP growth, particularly in developing regions, is crucial for improving life expectancy and shaping future global economic stability.
