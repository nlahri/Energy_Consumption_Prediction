# Energy_Consumption_Prediction

This project's objective is to utilize time series forecasting to predict the hourly energy consumption for a city in Morocco called Tétouan.

## **Dateset:** 

The dataset we are using is related to the power consumption of three different distribution networks in Tétouan, located in northern Morocco. The power consumption data for this project is collected and provided by Amendis, a public service operator, through their Supervisory Control and Data Acquisition System (SCADA). The distribution network in Tétouan is powered by three zone stations: Quads, Smir, and Boussafou. Each of these stations supplies power to different areas of the city, creating three distinct target variables. The dataset comprises 52,416 energy consumption observations recorded in 10-minute intervals, spanning from January 1st, 2017, to December 30th, 2017. We focused on one distribution network for our analysis, choosing the one with the highest consumption to align with the area coverage.

Power Consumption of Tetouan City - UCI Machine Learning Repository 
https://archive.ics.uci.edu/dataset/849/power+consumption+of+tetouan+city


## **Problem statement:**

The problem we aim to address is twofold. First, given that Morocco heavily relies on non-renewable energy sources (64%), forecasting energy consumption can assist stakeholders in managing energy purchases and stock more effectively. Second, while Morocco plans to cut down on energy imports by boosting production from renewable sources, these sources, such as wind and solar, are not available consistently throughout the year. By comprehensively understanding the energy demands of the country, starting with Tétouan, we can better strategize and allocate these resources. Additionally, accurate forecasting can help mitigate the energy imbalance between generation and consumption, ensuring that vital resources are used efficiently and sustainably.In a real-world scenario, the findings from this project could be instrumental for energy planners and policymakers. Accurate energy consumption forecasts would enable more efficient energy resource management, maintain the supply and demand equilibrium, and support the integration of renewable energy into the grid. This could lead to cost savings, improved energy security, and a more resilient power system for Morocco.

## **Model Comparision:**
There is a model comparison table in the pdf file shared in the repository. It discusses the incremental process of going from one model to another based on observations at each level

## **Conclusion:**
We have developed an effective model, LGBM_CYC_EXOG_ALL, which achieves an error rate of less than 5% for 95% of the forecasted values. However, the model encounters higher errors during peak consumption hours, which occur consistently at the same time each day. Additionally, the residuals exhibit patterns that suggest the presence of unaccounted factors in the model. Incorporating new data columns to capture these patterns presents an opportunity for further enhancement and improved accuracy in future iterations.

## **Code files**

Energy_consumption_EDA.ipynb : All the preliminary data analysis 

Energy_consumption_modular_model.ipynb: Model building and comparison, final model and conclusion

## **Instruction to execute**

1. Set up the environment using requirements.txt 
2. Download the file and run
3. Data can be read directly from the web



