# DataManagementProject


## Project Outline

In the Data Management course, I was required to create a dataset to address a research question using scraping and API methods, optionally integrating existing data for comprehensive analysis and store the dataset in a NOSQL DataBase. The aim of my project was to examine the potential **relationship** between a **car's price** and its **safety rating**, exploring whether consumers are willing to pay a premium for a safer vehicle.

**Technologies used:** *Python, Pandas, MongoDB, Selinium, BeautifulSoup Matplotlib, Seaborn.*

## How  
I scraped the data from two websites using Selenium and BeautifulSoup

- From [automoto](https://www.automoto.it/) I scraped the car's price:
  - I decided to scrape the price only of new cars otherwise I would have introduced bias by considering the usage of a car which has a great inluence on its price;
  - I took basic configuration's price again to avoid major bias by considering configurations with options that do not impact the safety of a car  
 
- From [Euro NCAP](https://www.euroncap.com/en) I scraped the safety ratings

After scraping the data it was important to clean and standardize the data itself to perform the merge between the two datasets. 

## Plots and Conclusions

![image](https://github.com/marta-brasola/DataManagementProject/assets/72508540/3e795769-ff3a-40c2-bfed-5f56f100bfad)
![image](https://github.com/marta-brasola/DataManagementProject/assets/72508540/1d72e2f0-eeba-49f3-b7bf-eab1301e3aba)

In this case, it's evident that the data is not evenly distributed. Most of the cars are classified with 5-star safety ratings, and within this category, there is a high variability in prices.
To better analyze the relationship, I calculated the average safety statistics and created a scatter plot to illustrate the connection. While the relationship is not strictly linear, the correlation coefficient between the two variables is approximately 40%. To explain the relationship between these two variables more comprehensively, more detailed analyses and the inclusion of additional factors in the model would be necessary.
This suggests that safety ratings play a role in determining car prices, but the relationship is influenced by various other factors that require a more in-depth investigation. Further analysis with a richer dataset and a more extensive set of variables would provide a clearer understanding of this complex relationship.

![image](https://github.com/marta-brasola/DataManagementProject/assets/72508540/f1f05914-514a-4ca5-bfc1-04986cb4b0ff)
![image](https://github.com/marta-brasola/DataManagementProject/assets/72508540/7f2851e6-fe8d-4737-b304-5f588705bbaf)

This represents the distribution of minimum and maximum prices for different trim levels. As one might expect, the maximum price exhibits greater variability compared to the minimum price. While the minimum price also includes some outliers, they are fewer in number compared to the outliers in the maximum price range.

To conclude, after collecting, cleaning, integrating, and analyzing all the data, the relationship between a car's safety test and its price does not appear to be very strong. However, it's important to note that considered the limited amount of data I have been able to gather, it would indeed be valuable to expand the dataset and incorporate additional factors that influence car prices. This expansion could include historical sales data for car models, other characteristics of the model or brand in general, and even an analysis of used cars. By collecting more data points, a more comprehensive analysis can be conducted, enabling a more meaningful understanding of the factors that impact car prices.

