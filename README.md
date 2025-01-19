Outlier Detection in Zamfara State Presidential Election Data Using Geospatial Analysis

Definition

An outlier is a data point significantly different from other values in a dataset. These deviations can be much higher or lower than the norm, often signaling irregularities or errors.

Context

In a recently concluded election in Zamfara State, Nigeria, the Independent National Electoral Commission faced widespread allegations of vote manipulation and irregularities. These claims raised questions about the integrity of the results, prompting the need for a data-driven investigation into potential anomalies at the polling unit level.

Objective

To identify polling units in Zamfara State where voting results deviate significantly from their neighboring units. The analysis aims to detect potential irregularities or influences by leveraging geospatial data and voting patterns.

Dataset

Source: Zamfara State dataset (ZAMFARA_crosschecked_1.csv).

Scope: 12 Local Government Areas, 70 Wards.
Parties Analyzed: APC, PDP, LP, NNPP.

Vote Counts:
•APC: 15,190
•PDP: 8,218
•LP: 34
•NNPP: 156

Methodology

1️⃣ Data Collection

Retrieved the longitude and latitude of each polling unit using the Google Geocoding API.

2️⃣ Calculating Outlier Scores

Calculated the mean and standard deviation of votes for each polling unit relative to its neighbors.
Computed the outlier scores to quantify deviations from expected patterns.

3️⃣ Identifying Outliers

Applied a threshold of 1 to the outlier scores to flag polling units with significant deviations.

Insights

Top Outliers Identified:

1️⃣ SABON GARI / MUHDA PRI SCH

Outlier Score: 8.320158

Closest Polling Units:
•BAGEGA II / MAKARANTA
•KATAFANA
•DAN FAGE
•ST UNGAR MAGAJI / PRIMARY SCHOOL AREA

2️⃣ DAMRI I / MODEL PRIMARY SCHOOL

Outlier Score: 4.70070

Closest Polling Units:
•SHIYAR TUDU PRIMARY SCHOOL
•BUKKUYUM PRIMARY SCHOOL
•KARTAWA

3️⃣ TABKIN BUSAU IV / N.D.L.E.A

Outlier Score: 3.856274

Closest Polling Units:
•BUKKUYUM PRIMARY SCHOOL
•ABARMA PRIMARY SCHOOL
•SHIYAR DANKADU II / KYALETA

Key Observations:

SABON GARI / MUHDA PRI SCH recorded the highest outlier score, suggesting possible voting irregularities.
BUKKUYUM PRIMARY SCHOOL appeared as a neighboring unit to two of the top outliers, raising further concerns about its results.

Scatter Plot Analysis:

The PDP and NNPP parties exhibited the most outliers, hinting at potential voting anomalies favoring or impacting these parties.

Conclusion

The geospatial analysis of the Zamfara State presidential election data highlighted significant outliers that may indicate voting irregularities. The findings provide a foundation for further investigations to validate the integrity of the results.

Explore More:

Visualizations and detailed calculations can be found in the Outlier Detection in Election Data Using Geospatial Analysis.ipynb notebook.





