# data-512-a1

### Goal: 
The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through September 30 2017.

### Licence of Source Data
Source data falls under the MIT licence.
Link: https://wikimediafoundation.org/wiki/Terms_of_Use/en#Our_Terms_of_Use


### Relevant APIs:

For this project, we used the APIs provided by wikipedia.
1. The legacy Pagecounts API 
   Documentation - https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts
   Endpoint - https://wikimedia.org/api/rest_v1/#!/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end
   
2. The Pageviews API
   Documentation - https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews
   Endpoint - https://wikimedia.org/api/rest_v1/#!/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end
 

### Final Dataset decription
For each month, year - the dataset provides the pagecount and pageviews at an accestype level (desktop/mobile) as well as an overall level

COLUMNS:
year - 2008 to 2017  
month - 1:12 from Januray to December  
pagecount_all_views - all page counts in month, year  
pagecount_desktop_views - dekstop page counts in month, year  
pagecount_mobile_views - mobile all page counts in month, year  
pageview_all_views - all page views in month, year (remove crawlers)  
pageview_desktop_views - desktop page views in month, year (remove crawlers)  
pageview_mobile_views - desktop page views in month, year (remove crawlers)  
  
### Notables

1. Pagecount data was missing for mobile site from 2008 to 2014. This is probably because wikipedia is currently not exposing these results to us.

 

