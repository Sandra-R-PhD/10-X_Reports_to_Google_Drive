# 10-X_Reports_to_Google_Drive  CC-BY-4.0 License
R code to copy select 10-X report files to your main Google Drive folder for text / sentiment analysis. 

Suggested citation
DOI: https://zenodo.org/badge/103856848.svg
Creative Commons License CC-BY-4.0

Recommendations for improvement can be directed to: Sandra.Rolnicki@hawk.iit.edu

# Description of files:
10X_Code_To_Share_v1.R --> Contains R code and references relevant R packages (googledrive and rlist)

PathExampleFile.txt --> Used to generate a list of file directory paths where the 10-X reports are stored. This sample file has each quarter as a subfolder of each year, as this is how they will unzip from McDonald's files (see note below on the original source of the 10-X report files)

CIK_List_Sample.txt --> Used to generate a list of "10-X" reports to pull by specifying the "pattern" that will be used by R to identify the files

# Notes on What This Code Does:
Zipped 10-X reports that have undergone "Stage One Parse" have been made available by the University of Notre Dame on their Software Repository for Accounting and Finance
http://sraf.nd.edu/data/stage-one-10-x-parse-data/

The web page at the link above includes a link to a Google Drive that holds all of the 10-X reports zipped by year and by quarter
Thanks to Professor Bill McDonald and his team for sharing these files!

Props to the creators of "googledrive" package for R! This would not have been possible without their elegant solution!
http://googledrive.tidyverse.org

The "rlist" package was also quite helpful!
https://renkun.me/rlist/

Note: In order to extract files from McDonald's zip files (and execute the steps detailed in the R code), you need to download the files to your computer (or server) and extract the files there.

There is a 3rd party app to unzip files in Google Drive. If this is used, the code can be modified to call your Google Drive folder rather than a local directory.
https://productforums.google.com/forum/#!topic/drive/s23OpZOTsq0
