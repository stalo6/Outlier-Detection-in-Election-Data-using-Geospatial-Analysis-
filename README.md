Outlier Detection in Zamfara State Presidential Election Data using Geospatial Analysis 

Definition:
An outlier is a data point significantly different from from other data points in a dataset.The difference can be much higher or lower than the other other values.

Context: 
In a recently concluded election, the Independent National Election Commission faced numerous legal challenges regarding the integrity and accuracy of the election results.Allegations of vote manipulation and irregularities have been widespread, prompting a thorough investigation into the matter.

Objective:
 The goal is to identify polling units in Zamfara State, Nigeria where voting results deviate significantly from neighbouring units, indicating potential influences or rigging.We aim to detect outliers that may indicate irregularities by analyzing the geospatial data and voting results.

Data Overview:
•Scope -12 Local Government Areas ,70 wards
•Parties involved -APC, PDP,LP ,NNPP
•Vote Counts -APC:15190 ,PDP:8218, LP:34, NNPP:156

Methodology:
1.Data Collection -Obtained longitudes and latitudes for each polling unit using Google Geocoding API.
2.Calculating Outlier Score- I calculated outlier score by first calculating the mean and standard deviation of votes for each polling unit from its neighbors then proceed to determining the outlier score.
3.Identifying outliers - I identified outliers by defining a threshold which I set to 1 to determine which polling units were outliers based on outlier scores.

Insights : 

The top outlier was SABON GARI / MUHDA PR SCH with an outlier score of 8.320158 with its closest polling units being BAGEGA II/ MAKARANTA , KATAFANA , DAN FAGE  and ST UNGAR MAGAJI / PRIMARY SCHOOL AREA.
The second top outlier was DAMRI I /MODEL PRIMARY SCHOOL with an outlier score of 4.70070 with closet polling units being SHIYAR TUDU PRIMARY SCHOOL, BUKKUYUM PRIMARY SCHOOL and KARTAWA.
The third top outlier was TABKIN BUSAU IV /N.D.L.E.A with an outlier score of 3.856274 with its closest polling units being BUKKUYUM PRIMARY SCHOOL, ABARMA PRIMARY SCHOOL, SHIYAR DANKADU II / KYALETA

Conclusion :

The SABON GARI / MUHDA PRI SCH record the highest outlier score (8.320158) indicating possible voting irregularities.
BUKKUYUM PRIMARY SCHOOL was among closest polling units to two of the top outliers indicating possible voting irregularities.
From the scatter plot below , PDP party and NNPP party had the most outliers indicating there must have been possible voting irregularities.



