## *Data Analytics (DataWarehouse and Visualization) project*

1. Description of a dataset

Chosen dataset - Global Terrorism Database (https://www.kaggle.com/START-UMD/gtd/version/3)

The Global Terrorism Database (GTD) is an open-source database including information on terrorist attacks around the world from 1970 through 2017 (except 1993). The GTD includes systematic data on domestic as well as international terrorist incidents that have occurred during this time period and now includes the exact number of 181 691 attacks.

The *.csv* file with the dataset contains 130 columns which provides numerous characteristics about terrorist attacks, which can be roughly grouped as follows:
- information about time and date,
- information about location, 
- information about tactics, 
- information about type of attack,
- information about perpetrators, 
- information about targets, 
- information about outcomes

After an initial analysis of the content of the dataset file it can be seen that there are some missing values among columns (f.e. in aproxdate or location column) and also some columns with very few values  (f.e. attacktype3) which should be considered and fixed during the preprocessing stage.

2. Preprocessing and cleaning data

Preprocessing and cleaning data tasks are very important part of the project as it is a set of
operations performed on the dataset to modify ambiguous data which can be a bottleneck to analytical results. It also helps in converting this raw data into a more meaningful, focused, interpretable and readable format.
The GTD dataset is incomplete, inconsistent, contains some errors, often missing attributes values, and outliers. Below data preprocessing tasks helped to resolve these discrepancies.

a) Manual analysis of the dataset and removing useless and irrelevant columns (analysis based on the official codebook - https://www.start.umd.edu/gtd/downloads/Codebook.pdf)
b) Calculating percentage of missing values for each column and removing columns for which calculated value is equal or greater than 80% (dimensionality reduction)
c) Analysis of empty values and their conversion
d) Dimensionality reduction caused by geographical changes

3. Relational database

4. Logical design

5. Visualization

As a last step of the project I used Tableau software to prepare visualizations from previously modified data.

a) victim characteristics dashboard

First dashboard is focused on victims that were killed or wounded during terrorist attack all over the world.
It allows searching through countries based on the specified number of victims. Then after choosing a particular country, it allows to check how many victims were in cities of this country (in descending order), how is the ratio of the different types of victims and how many victims were killed and wounded by specific type or types of weapon.

b) characteristics of attacks dashboard

Second dashboard is focused on the event of the attack itself.
It allows us to analyze how a particular type or types of attack has been changing over years in a specified country (or in general over the world if nothing is specified).
In addition it allows us to check the ratio of the different categories of attacks and how many properties were damaged during an attack in a specified country.
It also allows to perform above analysis only in a particular range of years or in particular range of number of attacks.


