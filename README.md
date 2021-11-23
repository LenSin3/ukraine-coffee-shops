# Segmenting Coffee Market in Ukraine

![Coffee Shop](https://github.com/LenSin3/ukraine-coffee-shops/blob/main/images/coffee_ukraine.PNG?raw=true)

Source: [Matador Network](https://matadornetwork.com/read/best-coffee-shops-kiev-ukraine/)

## Background

A fictitious company that owns a chain of coffee shops wants to identify the main segments in the coffee market and their key features. This information will help in the company's expansion effort into new markets, in this case Ukraine.

## Method

The project will follow the below steps:

- Read data.
- Transform data.
- Exploratory data analysis.
- Machine Learning.
   - Clustering with K-Means.
   - Cluster evaluation.
- Future work.
- Recommendations to management.

## Data

The data used in this project is obtained from [Datacamp's Career Hub repository](https://github.com/datacamp/careerhub-data) on GitHub.

## Example plots from Exploratory Data Analysis

![region vs place type](https://github.com/LenSin3/ukraine-coffee-shops/blob/main/images/regionVplacetype1.PNG?raw=true)

Varying Region with Place type we can tell there are more Coffee shops in Lviv followed by Odessa and Kharkiv. Shops labelled cafe are the the second most represented coffe shops with heavy presence in Khirvoy Rog and Dnipro.

![region vs price range](https://github.com/LenSin3/ukraine-coffee-shops/blob/main/images/regionVpricerange1.PNG?raw=true)

Prices between 10 and 100 dollars are the most common across all regions. Mariupol and Kiev are the only 2 regions that have shops with prices below 10 dollars while Poltava, Khrivoy rog and Dinipro are the three regions with prices above 100 dollars.

![reviews ratings delivery](https://github.com/LenSin3/ukraine-coffee-shops/blob/main/images/reviewsratingdine1.PNG?raw=true)

Coffee shops have the most reviews and among the highest rated. The highest and lowest rated is cafe but again they are the lowest rated. Of interest is that shops with prices above 100 dollars the not among the highest rated.

## Clustering of Coffee Shops by Region

KMeans clustering algorithm from Scikit Learn library is employed for the cluster analysis.

![elbow curve](https://github.com/LenSin3/ukraine-coffee-shops/blob/main/images/elbow_curve.png?raw=true)

The inertia plot indicates that a cluster of 4 will be ideal to segment current market.

## Future Work

- An improvement to the model will be to get rid of outliers and see how many clusters will be suggested.

- Hierarchical clustering will aid in showing progression of clusters as they merged.

## Recommendations to Management

- Segmenting the market into 4 regions is a good start for expansion into the coffee market in Ukraine.

- To be competitive, management must match price with shops that price products between 10 and 100 dollars.

- Opening a stand alone Coffee shop or Cafe will appeal to more customers than if the shops are to be opened in store, restaurant or coffee stand.

- More data will help in developing high performng models which in turn will aid management in better decision making.

- Variables like demographic and socio-economic status of the locations will also help in determining ideal areas to expand to.

## Dependencies

- Numpy 1.19.2
- Matplotlib 3.3.2
- Pandas 1.1.5
- Seaborn 0.11.1
- Scikit -Learn 0.23.2

## Notebook

- ukraine_coffee_shops.ipynb

## Environment

- python 3.6.12
