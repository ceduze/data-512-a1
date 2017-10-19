# data-512-a1
Assignment 1 template. See: https://wiki.communitydata.cc/HCDS_(Fall_2017)/Assignments#A1:_Data_curation

### Goal of this Project
The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through September 30 2017. I combine data Wikipedia traffic from two different Wikimedia REST API endpoints into a single dataset, perform some simple data processing steps on the data, and then visualize the data.


### License
Under MIT License (see license file)
CC-0
This data was provided by Wikimedia Foundation and can be found at the URLs below (API).

### APIs
[Legacy Pagecounts API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)  
[Pageview API](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews).


### Output Columns
**year (YYYY)**
4 digit year

**month (MM)**
1-2 digit month

**pagecount_all_views (num_views)**
Sum of all pagecount (legacy api) views

**pagecount_desktop_views (num_views)**
Count of all pagecount(legacy api) desktop views

**pagecount_mobile_views (num_views)**
Count of all pagecount(legacy api) mobile views

**pageview_all_views (num_views)**
Sum of all pageview (current api) views

**pageview_desktop_views (num_views)**
Count of all pageview (current api) Desktop views

**pageview_mobile_views (num_views)**
Count of all pageview (current api) moboile views. Sum of mobile-app and mobile-web.


### Other Issues
For rows where we do not have data available we leave the values as NaN. This is important if you plan to add columns. 

