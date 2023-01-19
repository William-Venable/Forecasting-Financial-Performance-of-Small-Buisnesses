![LB   Sons_2](https://user-images.githubusercontent.com/109354592/210472331-776fcdfd-617b-4fc3-98a9-8113439ff8b8.png)


# Forecasting Financial Performance of Small Business

## Project Overview
The purpose of this project is to determine the financial viability of a small business. We have an understanding that small businesses go to accounting firms with fears about going under, however, by the time the firm realizes that the company is flat they’ll notify the business that it’s too late. The intent of this project, is to be able to use machine learning for any small business with a simple exchange of data, our main focus will be LB & Sons with a potential to expand the data model to other small business entities. 

Jerry Barron, Vice-President of LB & Sons, has provided a dataset to help determine:

<ins>Questions we would like to answer with our machine learning model
  
1.	<ins>Future financials of the business
2.	<ins>Plateau date, if any, of the business
3.	<ins>Forecasted future of the business

## Website
Please click the link to learn more about **[LB & Sons](https://lbsons.com/)**
  
![LB   Sons_1](https://user-images.githubusercontent.com/109354592/210474611-73d80216-56cf-4942-b1e2-e016d5ea19d7.png)

## Resources
* [LB_Forecast_Cash_1.csv](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/868a1601c7760b9ab84af13c4cfac5e3cb98570e/Resources1/Resources/csv/LB_Forecast_Cash_1.csv)
* [LB_Forecast_Rec_1.csv](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/868a1601c7760b9ab84af13c4cfac5e3cb98570e/Resources1/Resources/csv/LB_Forecast_Rec_1.csv)
* [LB_Sales.csv](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/868a1601c7760b9ab84af13c4cfac5e3cb98570e/Resources1/Resources/csv/LB_Sales.csv)

## Technologies Used
  To perform our analysis, we had to determine which machine learning tool we were going to use.  We referenced scikit learn (Choosing the right estimator), which pointed to regression as our best choice.  The dataset was less then 100,000 samples but more then 50 samples.  Based on the cheat sheet below we decided to start with regression and expand to other models to experiment.
  
 ![scikit learn](https://user-images.githubusercontent.com/108476566/213287819-2c7c09da-891a-4d22-9ba2-3ca8e4833882.png)


  
 ## Dependent and Independent Variables
 Machine learning is based on the cross-analysis of dependent and independent variables.  The dependent variable (y) is the output we are wanting to predict and the independent variable(X) is an input that impacts the dependent variable(output).  The goal for the project was to find the independent variable(X) affect the dependent variable(y).
 
 To predict financial stability, we used supervised learning analyzes.  Our focus was on Cash and Receivables.  Cash is an important asset in the company as without substantial Cash it is very difficult to run a business.  The business needs cash to meet payroll demands, materials for current and future jobs, equipment repairs, supplier and operational expenses.  Without Cash, a company can quickly find themselves in large amounts of debt.  Construction companies are known to finance just about everything from payroll, to equipment, to the actual current job.  This is where a construction company can get into trouble.  Financing all your cash needs could make your company bankrupt very quickly.  Although, it is very possible to finance everything, it is not the way LB&Sons functions as a business.  LB&Sons follows the ideas of our grandparents, "If you dont have the money in hand as Cash, probably should not purchase".  Wether that is payroll or any other items.
 
 ##Linear Regression
 We started out with Linear Regression on both Cash and Receivables.  
  
  
      
    Finally, we located a time series mode, we had heard about and decided to give that a try.  We ended up using prophet (Time Series Model) and it was most accurate when compared to actual numbers.  Please see our work at Cash Estimate (Jupyter File), Cash Forecast Linear Regression, Cash Regression, Decision Tree Classification, Decision Tree for Regression, Linear Regression Beginners Guide and Linear Regression.
  
* [Linear Regression Beginners Guide.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/8647947c069d2f8f686af907b8060808b34e75b8/Resources1/Resources/ipynb/Linear%20Regression%20Beginners%20Guide.ipynb)
* [Linear Regression.ipynb ](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/9bdf2eca32dd13c20cf3a1339dd08bdf7fadde42/Resources1/Resources/ipynb/Linear%20Regression.ipynb)
* [Cash Forecast Linear Regression Best R2 score.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/9bdf2eca32dd13c20cf3a1339dd08bdf7fadde42/Resources1/Resources/ipynb/Cash%20Forecast%20Linear%20Regression%20Best%20R2%20score.ipynb)
* [Cash Estimate.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/9bdf2eca32dd13c20cf3a1339dd08bdf7fadde42/Resources1/Resources/ipynb/Cash%20Estimate.ipynb)
* [Cash Regression.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/79d16eb0d1df2fc81b7b207620bbbffb6aba5031/Resources1/Resources/ipynb/Cash%20Regression.ipynb)
* [Decision Tree Classification.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/e817ee27dc31f6ca3e247a381255d286fbce7231/Resources1/Resources/ipynb/Decision%20Tree%20Classification%20LB.ipynb)
* [Decision Tree for Regression.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/e817ee27dc31f6ca3e247a381255d286fbce7231/Resources1/Resources/ipynb/Decision%20Tree%20for%20Regression.ipynb)
* [LB Cash Prophet.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/0c2a20e9f583adbc435f5e2ca552f18a9953e026/Resources1/Resources/ipynb/LB%20Cash%20Prophet.ipynb)
* [LB Receivables Prophet.ipynb](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/0c2a20e9f583adbc435f5e2ca552f18a9953e026/Resources1/Resources/ipynb/LB%20Receivables%20Prophet.ipynb)


## Database
Using the years of data, spanning from 2021-2022, within the CSV files (Cash Flow, Receivables, and Sales) provided by Jerry from LB & Sons, we implimented the files into Tableu. We created four main graphs/tables to depict the Forecasts and recievables of cash for LB & Sons.

We will be breaking down each of the graphs/tables within our [Tableau file](https://github.com/William-Venable/Forecasting-Financial-Performance-of-Small-Buisnesses/blob/main/Financial_Perf_Dashboard/Financial_Performance.twbx) in the points below:
  
  - <ins>Forecast and Receivable
  
    - We have two main bars, Forcasted Receivables and Receivables. The forcasted receivables is the total sum of total forcasted receivables over the past two years within the CSV files, as well as the receivables being the sum of total receivables within the files.
   
 ![Forecast   Receivables](https://user-images.githubusercontent.com/109354592/211960376-82bde994-1007-4457-a8da-3ece2276474e.png)
    
  - <ins>Forcast and Receivable by Week
  
    - This table is just our previous Forecast and Receivable table but broken down by week. Anywhere that there is a null for the dates is a week that LB & Sons did not get any receivables.
    
 ![Forecast   Reveivables by Week](https://user-images.githubusercontent.com/109354592/211960418-e2e86797-f461-48f1-9bfe-47cf006c0d1f.png)

  - <ins>Sales by Week
  
    - This graph is a depiction of the total number of sales within each month over the past two years. We can see that during the Spring (April) going into the Summer (June), LB & Sons received the most amount of sales.
    
 ![Sales by Week](https://user-images.githubusercontent.com/109354592/211960500-91fc3be3-a2a5-4712-9658-7a54a9c8f400.png)

  - <ins>Forecasted Cash and Receivable
  
    - Within the graph, we have two lines, our Forecasted Cash (Blue line) and Actual Receivables (Orange Line). This clearly depicts a breakdown of the total amount of revenue received in 2022.
    
![Forcasted Cash   Receivables](https://user-images.githubusercontent.com/109354592/211960557-b18c7676-829c-4f93-8760-5087550bd7e2.png)

## Machine Learning Model

**Facebook Prophet** - https://facebook.github.io/prophet/

<ins>What is Facebook Prophet?
  
Prophet is a forecasting procedure implemented in R & Python. Prophet is fast & provides automated forecasts that can be tuned by data scientist & analysts.
  
It shows a time series data based on an addictive model where non-linear trends are fit with yearly, weekly, and daily seasionality, plus holiday effects. It works best with time series that have strong seasonal effects and several seasons of historical data. 
  
Prophet is open source software released by Facebook’s Core Data Science team. It is available for download on CRAN and PyPI.

Prophet is: `Accurate and fast`, `Fully automatic`, `Turnable forecast`, & `Available in R or Python`   
  
## LB & Sons Analysis

<ins>Description and Analysis of our data looking over LB& Sons
  
<ins>What are some possible improvements we could make?
- `How can our model be improved on?`
  
  ![LB   Sons](https://user-images.githubusercontent.com/109354592/210474480-6c687ea1-56ba-4134-9e81-bfbeabb5dd42.png)

  


  
