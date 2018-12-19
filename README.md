# Does basic house information reflect house's description?
========================================

Joanna Broniarek, Vikranth Ale, Matteo Cavalletti

![houses-image](https://st.ilfattoquotidiano.it/wp-content/uploads/2018/04/03/Articolo_Ripresa-Mercato-Immobiliare.png)

**The aim of this project was to perform a clustering analysis of house announcements in Rome from Immobiliare.it.**

## Data Source

## Steps
1. Creating two datasets (**Information Dataset and Description Dataset**) according to data scrapped from websites. Retrieving at least 10000 announcements.

2. Clustering the house announcements using **K-mean++ method**.In order to choose the best number of clusters per dataset **the Elbow method** was used.

3. Comparison among clusters. Do both datasets will lead to similar clusters?
  + Finding similar clusters according to the Jaccard-Similarity. 
  + Returning the 3-most similar couples of clusters (information clusters vs description clusters)
  + Creating Wordclouds of house descriptions. The represented words extracted from the description of the houses that are in the relative couple.

## Jupyter Notebooks Descriptions
1. **Main_HouseClustering** - main notebook, where most of the analysis is contained
2. **TFIDF_matrix** - notebook for generating TFIDF matrix needed for Description Dataset.

Some functions used in analysis was located in the external files : collect_data.py, functions.py.

Folder DataFiles contains files, which were created and used during the analysis.

### Technology
Python 3.6.4 (beautifulsoup, sklearn, wordcloud)
