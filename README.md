# Project_Ecommerce_BI
Pacmann Project - Data Analytics Ecommerce

<h1>Sales-Marketing-Business Dev Ecommerce Dashboard</h1>

<h2>1.	Background</h2>

As a new BI Analyst at a new founded ecommerce company, we’re analyze to be a part of successful operations, the company need to monitor their entire activity. There are plenty of rich data in internal system consist of sales data (sales actual data, customer and seller data, review data etc), marketing data (promotion and campaign data, profile customer data) and business development data (ab testing data). So, we’re proposed a comprehensive dashboard to C-level and each team member in sales, marketing and business development.

<h2>2.	Objectives</h2>

<h3>i) Vision</h3>

Providing organizations with the power to know with data visualization. Make the lives of our CEO, Sales and Marketing and BD team better through providing an insightful data.

<h3>ii)	Goals</h3>
We’re setting up our goals based on each team and functions:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;A. Sales: Providing information related to sales and operations performance such as order, profit, review and seller information

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;B. Marketing: Segmenting user and determining the effectiveness of marketing and retention of customer

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;C. Business Development: Determining which version of landing page is better based on A/B testing

<h3>iii)	Initiatives</h3>

Creating a Dashboard to monitor and improve sales, marketing and business development based on each team goals. So, our teams can see their performance.

<h3>iv)	Personas</h3>

o	High Managerial Level for Quick update and actions

o	Sales and Operational Team: to drill down and investigate sales

o	Marketing Team: to see and analyze effectiveness of marketing and retention

o	Business Development Team: to get a conclusion for landing pages based on data


<h3>v)	Features</h3>

o	About Us: Will show you the dashboard homepage and overall status for every key matrix

o	Sales Overview: Will show you the sales general information from total sales, total order growth size etc

o	Sales Review: Will show you the information of review segment, in general it will show customer feedback and proportions

o	Sales for Seller: Will show you the overall seller performance and and rank for seller

o	Marketing dashboard: Will show RFM analysis and also cohort analysis to see our customer engagement

o	AB Testing: Will show the result of AB testing and suggestion for next action based on data



<h2>3.	Overview dan Process:</h2>

<h3>a.	Proses</h3>
<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture1.png" width="350" title="hover text">
</p>

i.	Extracting the data

On this case, because of we’re using an extracting data sample so first is downloading the data from their data source. But in the future, it’s better if we’re connecting the data pipeline from ERP – Database (SQL) and put it in python to analyze.
Data is having several information to analyze the data. Below is list of data to create a comprehensive dashboard as we’re sharing in previous section.

1.	Sales Data:

a.	Order list dataset

b.	Order item dataset

c.	Order review dataset

d.	Order customer dataset

e.	Order seller dataset

f.	Order product dataset


<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture2.png" width="350" title="hover text">
</p>

2.	Marketing data

3.	BD Data – AB testing data


ii.	Data Cleaning and Data processing

After the data collected, data marketing is ready to use on tableau. While data sales need some cleaning and data AB testing need to analyze more in python script.

1.	Data Cleaning – Sales Product

Data here is quite straightforward, the data is clean enough and we need to do cleaning on 2 parts, translating the product name and also mapping state name into province name.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture3.png" width="350" title="hover text">
</p>

a.	Use google trans==3.1.0a0 dan import Translator

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture4.png" width="350" title="hover text">
</p>

b.	Translate column name and data in product category name

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture5.png" width="350" title="hover text">
</p>

2.	Data Cleaning – Regional mapping

Currently the data is not referencing a right area, so we need to search from internet and mapping those state code into state name

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture6.png" width="350" title="hover text">
</p>

3.	Data wrangling - AB testing

AB testing test will be done in python completely and the result will be simulated in tableau part.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture7.png" width="350" title="hover text">
</p>
 
 a.	Visualizing result, To calculate some basic statistics to get an idea of what our samples look like.
 
 <p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture8.png" width="350" title="hover text">
</p>

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture9.png" width="350" title="hover text">
</p>

b.	Testing the hypothesis and drawing conclusions, To calculate -value (i.e. z-test) using normal approximation with very large sample.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture10.png" width="350" title="hover text">
</p>

c.	Daily dataset analysis, actually almost same process as previous process but we’re analyzing the data in daily basis

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture11.png" width="350" title="hover text">
</p>

iii.	Data Visualization

After the data is clear both AB testing and sales, we need to input those data in the dashboard tableau and do some analysis in tableau part.
 
<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture12.png" width="350" title="hover text">
</p>

1.	Data Marketing – RFM Analysis
While other dashboard (sales and ab test) is done in python, for RFM analysis calculation is happened in tableau. We’ll create analysis based or Recency (last time they buy our product), Frequency (how many times they order our product), and Monetary (total sales). After that we’re grouping them into several group based on RFM score.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture13.png" width="350" title="hover text">
</p>

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture14.png" width="350" title="hover text">
</p>

<h3>b.	User Flow</h3>

After the dashboard is finished and published publicly, here is the userflow that we hope will be run by the user. With this userflow, it will answer some of the questions that have been stated in the previous sub-chapter.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture15.png" width="350" title="hover text">
</p>

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture16.png" width="350" title="hover text">
</p>

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture17.png" width="350" title="hover text">
</p>

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture18.png" width="350" title="hover text">
</p>

<h2>4.	MVP Demonstration</h2>

With the data clean and clean and then processed properly and according to the problem we stated earlier, here is an MVP demonstration to explain the features and functions. Here is also attached the dashboard link for further testing.

https://public.tableau.com/app/profile/a.roof.tito.anggoro/viz/PACMANNPLBI2-JAVATEAMECOMMERCE/E-CommerceDashboard

<h3>a. Homepage Dashboard</h3>

An opening page when you’re accessing the dashboard, shows you dashboard title and your username (means you’re already login correctly)

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture19.png" width="350" title="hover text">
</p>

<h3>b.	About us Dashboard</h3>

Showing how to use dashboard and which area (sales/marketing/Abtest) you want to explore. In this page shows overall dashboard performance (sales, order,etc)

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture20.png" width="350" title="hover text">
</p>

<h3>c.	Sales dashboard – Overview</h3>

Showing overall performance in sales data, from monthly sales, forecast, sales per area (region, product, top seller and top customer) and their growth

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture21.png" width="350" title="hover text">
</p>

<h3>d.	Sales Dashboard – Review</h3>

Showing review category and performance, it has review proportions, indicator and trend also.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture22.png" width="350" title="hover text">
</p>

<h3>e.	Sales Dashboard – Seller</h3>

Showing your seller performance, we can check based on review, response and number seller per area

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture23.png" width="350" title="hover text">
</p>

<h3>f.	Marketing dashboard – Customer segmentation</h3>

Showing how you played with data correlation in several parameter and its impact to champaign result. Also break it down customer level based on RFM score.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture24.png" width="350" title="hover text">
</p>

<h3>g.	AB Testing</h3>

Showing a result of ab testing, based on the data processing on phyton on previous segment.

<p align="center">
  <img src="https://github.com/Marwin88/Project-Lab-BI-2-Pacmann/blob/main/data/picture/Picture25.png" width="350" title="hover text">
</p>


<h2>5.	Analysis and result</h2>

Based on dashboard in previous segment, we can get some conclusions from the data and we can split it into several segment as per below.

a.	Beauty health, watches and furniture is our strong point on our sales, that 3 products can generate 28% from total sales, and our sales is growing if we compare 2017 and 2018 on same period

b.	Review in average is 4.1 with mostly focus on service, and if we see reviews is getting better every year

c.	Late delivery mostly happened from sau paulo in same city. The main reason is because most of the order is coming from this city

d.	On marketing side, high class customer group having overall high CVR and high champaign accepted. Most of high-class customer is segmented as champions by 20% and at risk by 19%

e.	On AB testing, because of P value 0.21 and it’s higher than alpha (0.05) so it fails to reject H0. Resulting the two pages (old and new) is not significantly different



<h2>6.	Reference</h2>

AB Testing Data - https://docs.google.com/document/d/1V7O6xiJ0wH5h3ddBK4Ji0vcD_6DNuXuKWb-yxRw28Ww/edit

Marketing Data - https://docs.google.com/document/d/1OCgfp8fGf9QSAEVtb8qNWspVGORqNWhx-uEy3KoD4Yc/edit

Sales Data - https://docs.google.com/document/d/1v33dd7tNS6pYoUXp32GO1YyW1LpxuvDMuFJmKOYJdsY/edit

