# Senior_Project
This GitHub will hold the senior project for Iyana Jones &amp; Coreen Mullen for Senior Seminar, Spring 2025.

The senior project was to create a hot-spot analysis map of traffic accidents in North Carolina using different clustering algorithms.

To access the code for this project, unzip the folder and use an IDE of your choice to begin running the code using Python.

The Raw_Data folder holds the folders with the FARS 2022 and 2021 datasets in the original folders.

The accident_analysis_html_maps folder holds the output files of plot.py.
- By double-clicking on one of these html files a interactive map of the labeled county should appear with dots representing where the accidents happened in the two different years ( without clustering ).

The methods.py file holds the Principal Component Analysis, Silhoutte Method, and the Elbow method. It also prints results into the terminal for the k-means and dbscan k-value determinations based off the data. 

The preprocessing.py outputs filtered data from the original .csv files given from the Fataity Analysis Report of 2021 and 2022. 
- This file outputs the nc_accidents_2022.csv and nc_accidents_2021.csv hold the data for both datasets.

The distance.py file outputs the county_distance_matrices folder which contains the distance matrix for all the counties. 
The distance_db.py is dependent on the distance.py. It uses the matrices to get a value for DBSCAN to use in its clustering. It outputs a folder (county_dbscan_labels) with the results for each county.
  - To read the files in the county_dbscan_labels, the key is :
    -1: Considered noise (not assigned to any cluster).
    0: This point belongs to cluster 0 (the first cluster found by DBSCAN).
    1: This point belongs to cluster 1 (the second cluster found by DBSCAN).
*Note some files have only one cluster or 0 clusters which would include a file with all -1 values.

There are multiple csv files included in the code, the accident_2021.csv & accident_2022.csv have been filtered to include solely North Carolina.
The nc_accident_analysis_2022.csv and nc_accident_analysis_2021.csv are created by the methods.py and include the PCA, k-means, and DBSCAN values.
