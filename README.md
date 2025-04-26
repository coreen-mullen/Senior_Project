# Senior_Project
This GitHub will hold the senior project for Iyana Jones &amp; Coreen Mullen for Senior Seminar, Spring 2025.

The Raw_Data folder holds the folders with the FARS 2022 and 2021 datasets in the original folders.

The accident_analysis_html_maps folder holds the output files of plot.py.
- By double-clicking on one of these html files a interactive map of the labeled county should appear with dots representing where the accidents happened in the two different years ( without clustering ).

The methods.py file holds the Principal Component Analysis, Silhoutte Method, and the Elbow method. It also prints results for the k-means and dbscan k-value determinations based off the data.

The preprocessing.py outputs filtered data from the original .csv files given from the Fataity Analysis Report of 2021 and 2022. 
- This file outputs the nc_accidents_2022.csv and nc_accidents_2021.csv hold the data for both datasets.

The dbscan.py outputs simular result as the plot.py where it takes the maps and divides them by county but it performs the DBSCAN clustering by county aswell and visualizes how DBSCAN would cluster the data.
