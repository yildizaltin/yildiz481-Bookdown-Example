# Regression Output Table Examples


This RMD file was one of the examples you worked through in 380. I'm including it in this example for a few reasons. First, you can see how RMD files that you used before as standalone RMD files to create standalone HTML output can be combined in a book using bookdown. Second, this file loads data using `read.csv("data/ceo.csv")`, serving as an example of how you will store all data in a "data" folder put in the main project folder. Third, this file provides examples of showing regression output side by side. 



Note: Generally it's a good idea to load your packages in a code chunk at the top rather than mixed in with the rest of the document. However, for this example I am going to load the packages  in the same code chunk where I use them so that you can see exactly what package is needed for specific functions.




The dataset `ceo.csv` has the following variables:
  
  Variable | Description
----------- | -----------
`salary` | 1990 compensation in dollars ($)
`age` | age of CEO in years
`comten` | years CEO with company
`ceoten` | years as ceo with company
`sales` | 1990 firm sales in $millions
`profits` | 1990 profits in $millions
`mktval` | 1990 market value in $millions

## Summary Statistics
The `stargazer` package provides an easy way to display summary statistics. You need the `result='asis'` codechunk option so that it displays the html table in the knit output file. The `warning=FALSE` and `message=FALSE` keeps it from displaying some of the messages it displays by default. One limitation of the table output is that it doesn't leave much space horizontally. This can be controlled by HTML options for cell padding in tables. 






































