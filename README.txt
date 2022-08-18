A web spider to scrape and extract information of listing foreclosure houses data in City Beijing at Jingdong Foreclosure and Ali Foreclosure, using Python package selenium, requests, pdfplumber and pyecharts.

1. scrape_data_at_Ali_Foreclosure & scrape_data_at_JingDong_Foreclosure:
use library selenium to select searching constraits and collect introductive info like titles, URLs and save them as a list in entry_url_list.csv.
then use library requests to download third-party price evaluation reports from this URLs, saved in ./Download_Files folder by every entry.

2. analysis_foreclosure:
use library pdfplumber to extract detailed information from downloaded pdfs and save them as parquet for further analysis.

3. geo:
use library pyecharts provided by Baidu Map to visualize data on interactive maps, presenting relationships beteewn longitudes, latitudes and prices.