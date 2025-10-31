# Statistical Data Analysis – AGH Project 1  

## Project topic  
**Assessment of the socio-economic development level of countries around the world**  

The goal of this project was to compare countries in terms of selected socio-economic indicators using two multivariate statistical methods: **linear ordering** and **cluster analysis**.  
The project was developed in **R** using the **RStudio** environment.  

---

## Project contents  

- **Projekt1.Rmd** – main file with R code, analysis, and interpretation (rendered to HTML)  
- **countries of the world.csv** – raw dataset  
- **countries_clean_scaled.csv** – cleaned and standardized dataset  
- **Charts and tables** – visualizations of distributions, correlations, rankings, and clusters  
- **Projekt1.html** – final report in HTML format  

---

## Data description  

The data come from the file *countries of the world.csv*, based on official U.S. government sources.  
They include socio-economic indicators such as:  
- GDP per capita  
- Literacy rate  
- Number of phones per 1000 inhabitants  
- Infant mortality rate  
- Birth and death rates  
- Industry and service shares in GDP  
- Climate  

The dataset is treated as **cross-sectional data** (countries compared at one point in time).  

---

## Methods used  

### Linear ordering  
Two techniques were applied:
- **Non-pattern method** – mean of standardized variable values,  
- **Pattern (Hellwig) method** – comparison of each country to an ideal reference country.  

Both methods produced very similar results (correlation r ≈ 0.98), confirming ranking consistency.  

### Cluster analysis  
Two clustering methods were used:  
- **k-means** (partitioning method),  
- **Ward’s hierarchical method**.  

The optimal number of clusters (k = 4) was determined using the **elbow method**.  
Both approaches resulted in a similar division of countries into four groups, representing different levels of socio-economic development.  

---

## Main findings  

1. The applied methods enabled a clear classification of countries by their level of socio-economic development.  
2. The two linear ordering methods (non-pattern and Hellwig) produced consistent results, confirming their reliability.  
3. Cluster analysis revealed four main groups of countries differing in development level.  
4. Highly developed countries formed a separate cluster, while less developed ones were grouped together.  
5. The results confirmed that socio-economic data effectively reflect global development disparities and can be analyzed using statistical methods.  

---

## R packages used  

`dplyr`, `ggplot2`, `readr`, `tidyr`, `scales`, `corrplot`, `factoextra`, `RColorBrewer`  

---

## Course

AGH University of Science and Technology in Kraków  
Course: *Statistical Data Analysis*  
