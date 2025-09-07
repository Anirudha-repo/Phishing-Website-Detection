# Data Files

This folder has the raw & extracted datafiles of this project. The description of each file is as follows:

* 1.Legitimate URLs,csv: This file has list of legitimate urls. The total count is 35,300. The source of the dataset is University of New Brunswick, https://www.unb.ca/cic/datasets/url-2016.html. 

* 2.Phishing URLs.csv: This file is downloaded from the opensource service called PhishTank. This service provide a set of phishing URLs in multiple formats like csv, json etc. that gets updated hourly. To download the latest data: https://www.phishtank.com/developer_info.php.

* 3.Feature_Extracted LegitimateURLs.csv: This file has the extracted features of the 5000 legitimate URLs which are randonmly selected from the 'Legitimate URLs.csv' file.

* 4.Feature_Extracted PhishingURLs.csv: This file has the extracted features of the 5000 phishing URLs which are randonmly selected from the 'Phishing URLs.csv' file.

* 5.Combined_URL_Data.csv: This file is nothing but a combination of the above two files. It contains extracted features of 10,000 URLs both legitimate & phishing.
