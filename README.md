# Customer_KPI

Extraction of Customer KPI from Business Articles and classifying them as Customer KPI or  Non-Customer  KPI  Documents.


### Algorithm:

**1) We read 300 PDF files and found the below Customer KPI keywords:**
```
* Net Promoter Score
* Customer Retention Rate
* Customer Profitability
* Customer Lifetime Value
* Customer Turnover Rate
* Customer Engagement
* SERVQUAL
* Customer Complaints
* Market Share
* Market Growth Rate
* Brand Equity
* Conversion Rate
* Customer Online Engagement
* Online Share of Voice
* Social Networking Footprint
* Klout Score
* Corporate Reputation
* DIFOT Rate
* Brand Attributes
* Customer Support
* Customer Attraction
* Customer Experience 
* First Contact Resolution
* Customer Callback
* Wait Time for Callers
* Customer Satisfaction
* Customer Loyalty
```

2) **Conversion of PDF to text**  
We used PDFMiner to convert PDF to text. Read all the PDF files record by record using PDFMiner. Wrote all those files to respective text files.

3) **Extraction of KPI from text**   
Made a list of all the extracted customer KPIs from various sources. Searched all the files to find customer KPIs in it. In this way, files were put into separate clusters, that is, Customer and Non-Customer KPI.

4) **Conversion to dataframe**    
With the help of Pandas library this task was completed.

5) **Classification of Documents**  
Output from the dataframe was converted into PDF and the Extracted Documents which contained Customer KPIs we manually classified them as Customer KPI or No.

6) **Writing out code for different Machine Learning algorithms**  
Multiple  Machine  Learning  algorithm  codes  were  such  as  AdaBoost,  Decision  Tree,  Random Forest, Neural Networks.  

7) **PCA with transformation**  
We used Principal Component Analysis for reducing the dimensionality of the data. It helps the machine learning algorithm to fit the data better as the learning parameter reduces and we can easily visualize the data.

8) **Testing Machine Learning Algorithms**  
Divided the dataset into test and train having 20% and 80% ratio respectively. Used different classifiers from SkLearn library.
Upon comparison, it was found that AdaBoostClassifier performed the best on the dataset provided. 
