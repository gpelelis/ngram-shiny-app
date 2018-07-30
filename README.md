# ngram shiny app
### A Shiny app built for analyzing the Search Terms report from AdWords.

![preview](https://i.imgur.com/s6vd7JO.jpg)

---
### Data Cleaning  

- Export Search Terms Report as CSV from AdWords  
&nbsp;  
- Delete first and last two rows from CSV  
&nbsp;  
![first two](https://i.imgur.com/gwV5DOF.png)
&nbsp;
![last two](https://i.imgur.com/8yENiAQ.png)
&nbsp;
- Make sure numeric columns are formatted as numbers
  - exact to two decimal points (eg. 1 -> 1.00)
  - remove currency and percentage signs (eg. $ and %)
  - no comma separators  
&nbsp;
- Your CSV has these columns
  - Search terms
  - Clicks
  - Cost
  - Conversions
  - Impr.

---
### Get Up & Running  

To run locally, clone the repo.
```bash
git clone https://github.com/beigebrucewayne/NgramShinyApp.git
```

Then, make sure you have R installed. The easiest way is to download from [CRAN](https://cran.r-project.org/).


Then, in the project directory start R
```
r
```
Then, in the r environment, type the following in order to install the packages. 
```
install.packages('shiny')
install.packages('tidytext')
install.packages('shinythemes')
install.packages('tidyverse')
install.packages('dt')
install.packages('wordcloud')

library(shiny)
```
Finally, execute the web app
```
shiny::runApp()
```
