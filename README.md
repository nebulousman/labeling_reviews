# labeling_reviews

Created as part of a CrowdDoing project to label reviews of medicinal products. The code selects samples to distribute for labeling, placing them into excel files. Excel provides data validation functionality to ensure consistency in labels. Returned files are then read and placed in a master dataframe which is appended as more labeled reviews are returned.

The output files from this repository are located at: Medicinal Foods/DataScience/Data Science Orientation/20200710-Scrapy_Data/Analysis/. They are:

* returned_labels_FOR_ANALYSIS.csv contains all labeled reviews except ones where all labels were null. Volunteers were instructed to skip reviews which were not about medicinal foods so they could be filtered out this way. 

* codedlabels_FOR_MODEL.csv cleans up further and contains review text and numeric codes of labels. All null values have also been filled. ID_allreviews_ index corresponds to index of allreviews.csv. To use read codedlabels_FOR_MODEL.csv and select ‘review’ plus the desired target variable column to perform classification task.

Both files are updated directly in the Crowddoing GoogleDrive by:
https://colab.research.google.com/drive/1WurJiUTK13xwZF6-PC53Ik8DXxuweEJ2
