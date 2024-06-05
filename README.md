# Predicting-S&P-500-Stock-Price
Utilizing Yahoo Finance's daily stock price data to predict the rise or fall of stock prices over the next 3 months.


•	Utilized tidyquant in R to pull Yahoo finance daily closing price of S&P 500 companies over span of 3 years.

•	Used Python to implement unsupervised machine learning techniques, identified distinguishing patterns in 20+ companies and used the insights to tune multiple supervised learning models including non-linear models.

•	Implemented time series decomposition to extract seasonal and trend components of each company and added it as new features to models, improving the overall accuracy of neural network model by 15%.


Variation of closing price relative to the first closing price for few stocks colored by sector. We can observe exponential change in closing price of TESLA stock compared to other.

![image](https://github.com/vedantkan/Predicting-S-P-500-Stock-Price/assets/68374993/c8d02be1-df01-4c39-b210-1c578a556ead)

Relative closing price for consecutive days are highly correlated. As we move farther the correlation starts decreasing.

![image](https://github.com/vedantkan/Predicting-S-P-500-Stock-Price/assets/68374993/2b502868-4ecf-42f4-b129-dccdd58758fd)

Using time series decomposition extracted trend component of the data. Performed PCA on the trend components. Additionally applied hierarchical clustering on first 10 PCA and after cutting the tree at appropriate point.

![image](https://github.com/vedantkan/Predicting-S-P-500-Stock-Price/assets/68374993/fcb2126a-92e2-483a-86cf-b871983d32b0)

Comparing model performance of several non-linear models. Adding the trend and seasonal components from time series decomposition increased model accuracy.

![image](https://github.com/vedantkan/Predicting-S-P-500-Stock-Price/assets/68374993/b46bdf42-8e3b-47d6-827c-78946de74161)

Created prediction grid using random forest model in order to visualize the trend of event with respect to inputs to understand model behavior to different inputs. We can see where the models finds it easy to predict vs what it finds difficult to distinguish between events. This gives us a better idea about the limitations of the model. 

![image](https://github.com/vedantkan/Predicting-S-P-500-Stock-Price/assets/68374993/b75ee729-061d-4017-8464-efd6e12f7736)


