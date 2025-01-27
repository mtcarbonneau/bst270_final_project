# BST270 Final Project

This repository has been created to meet the objectives of the Harvard BST270 final project.

# Objective 
Reproduce several figures in the FiveThirtyEight article [Marriage Isn’t Dead — Yet](http://fivethirtyeight.com/features/marriage-isnt-dead-yet/).

# To Run
The replication of the FiveThirtyEight analysis can be found as the R Markdown file `Final_Proj.Rmd` in the root of the repository. The project can be run entirely in base R and was created using the following specifications:

`R version 4.4.2 (2024-10-31)`
`Platform: aarch64-apple-darwin20`
`Running under: macOS Sequoia 15.1.1`

This notebook uses R Markdown and can be executed in [RStudio](https://posit.co/download/rstudio-desktop/).

## Getting Started
1. Clone the repository
2. Open `Final_Proj.Rmd`
3. Execute the notebook (top right corner of the screen: `Run` then `Run All`)

The notebook can be converted into a pdf using `Knit`. This pdf is included in the root of the folder: `Final_Proj.pdf`.

# Data

(Content revised from [FiveThirtyEight ReadMe](https://github.com/fivethirtyeight/data/tree/master/marriage) ).

This folder contains data behind the story [Marriage Isn’t Dead — Yet](http://fivethirtyeight.com/features/marriage-isnt-dead-yet/).

Source for all data is Decennial Census (years 1960 to 2000) and American Community Survey (years 2001-2012), via [IPUMS USA](https://usa.ipums.org/usa/cite.shtml).

Except in the divorce file, figures represent share of the relevant population that has never been married (MARST == 6 in the IPUMS data). Note that in the story, charts generally show the share that have *ever* been married, which is simply 1 - n. In the divorce file, figures are share of the relevant population that is *currently* divorced, conditional on having ever been married.

Relevant variable names are as follows. Number in variable names are age ranges, so `all_2534` is the marriage rate for everyone ages 25 to 34.

Header | Description
---|---------
`all` | Total (or all men/women in sex-specific files)
`HS` | High school graduate or less (EDUCD < 65)
`SC` | Some college (EDUCD >= 65 & <= 100)
`BAp` | Bachelor's degree or more (EDUCD > 100)
`White` | Non-Hispanic white
`Black` | Black or African-American
`Hisp` | Hispanic of any race
`nokids_all` | No own children living at home
`kids_all` | At least one own child living at home
