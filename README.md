# Employee-Retention-Analysis
Used logistic regression model in ML to predict the factors on which employees can be retained

First of all, to do the data analysis, we need data.
Dataset can be downloaded from: https://www.kaggle.com/datasets/giripujar/hr-analytics

After you have downloaded the data, read it thorugh the jupyter notebook and create a dataframe using pandas.

Analyze the dataset by considering for how many columns the "left" = 1 and "left" = 0.
Group the dataframe by left and take average of all attributes.
This gives us a clear understanding of which factors are responsible for employees "leaving" or "being retained".


![image](https://user-images.githubusercontent.com/73712335/222899877-eec85a2b-d2ac-4cf0-93ce-147b48d62d8d.png)

Some important factors are:
1.Satisfaction Level : Low in employees leaving the firm
2.Avg. Monthly hours : High in employees leaving the firm
3.Promotion in Last 5 Years : Employees who are given promotion are likely to be retained

Now one important aspect is left out i.e the SALARIES.
We plot a bar graph depicting fraction of employees leaving corresponding to their salaries

![image](https://user-images.githubusercontent.com/73712335/222900263-bca52af6-74f6-4846-8826-f68fc9b24f31.png)

Now we use dummy variables and OneHotEncoding to convert salaries from text to 1's and 0's.

Then we train the model using logistic linear regression.

![image](https://user-images.githubusercontent.com/73712335/222900447-32b6b50b-7d2a-4985-9330-da00073627f2.png)

Finally we find the accuracy of the Model.

![image](https://user-images.githubusercontent.com/73712335/222900462-e55fb9c5-a6cd-44ee-962f-ff61a7d6941f.png)







