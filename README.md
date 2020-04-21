# Monthly Crime Data

[Washington University Medical Center Redevelopment Corporation](http://wumcrc.com) is a partnership between BJC HealthCare and Washington University School of Medicine and works to improve the quality of life for the neighborhoods surrounding the medical campus. In order to achieve this goal in Forest Park Southeast and the Central West End , WUMCRC has invested millions of dollars toward regenerating the market for private investment in businesses and real estate, enhancing human and social service opportunities, and improving the level of physical and personal security.

One way we work to improve the level of physical & personal security is the analysis and distribution of crime data. The original source of the crime data is found here: <http://slmpd.org/crimereports.shtml>. If you have questions regarding the crime data visit <http://slmpd.org/Crime/CrimeDataFrequentlyAskedQuestions.pdf>.

In it's original form, the St. Louis Metropolitan Police Department (SLMPD) crime data is downloadable as a `csv` file. The data itself is also unorganized and challenging to work with. In an effort to simplify & reduce the time it takes to compile our reports, `r`, `tidyverse`, and `compstatr` are all packages that streamline and help our process. This project utilizes these resources for accessing and cleaning the data, with the eventual goal of automating the majority of our reports.

# To Reproduce this Analysis

1. You will need [R](https://www.r-project.org/), it can be downloaded from it's [website](https://cloud.r-project.org/).
2. You will also need [RStudio](https://rstudio.com/), it can be downloaded from it's [website](https://rstudio.com/products/rstudio/download/).
3. Download this repository and save it to your preferred working directory. 
4. Unzip the folder. 
5. Open the `monthly-crime-reports.Rproj` file with [RStudio](https://rstudio.com/).
6. Within [RStudio](https://rstudio.com/) open the following file - located in the [/source](https://github.com/wumcrc/monthly-crime-reports/tree/master/source) folder.
   * `data-creation.Rmd`
7. After opening the `data-creation.Rmd` review the `YAML`
   * The first section of an `R Markdown` document is called the `YAML`. The document title, author, date of publication, and other options for the entire document can be set in the `YAML`. The user can also set specific parameters to be referenced throughout the document. You can learn/read more about the `YAML` in an `R Markdown` document [here](https://r4ds.had.co.nz/r-markdown.html#yaml-header).
   * This section is important to note because there are parameters that you will need to change if you'd like to run this report for a different time frame. 
8. Make any appropriate changes to the `YAML`, reviewing the comments on lines 7 through 14. 
9. Run the `data-creation.Rmd` file first.
10. After running the `data-creation.Rmd` file open the other following files listed below. These are also located in the [/source](https://github.com/wumcrc/monthly-crime-reports/tree/master/source) folder.
   * `fpse-bot-cwe-mc-presentation.Rmd`
   * `sdb-dbp-we-vp-presentation.Rmd`
   * `ac-fp-lp-vd-presentation.Rmd`
11. After opening the files review the `YAML` sections for each of the files and make the appropriate changes.  
12. Once you've made your changes you'll want to `Knit` the following files. 
   * `fpse-bot-cwe-mc-presentation.Rmd`
   * `sdb-dbp-we-vp-presentation.Rmd`
   * `ac-fp-lp-vd-presentation.Rmd`
13. The automatic output (PowerPoint presentations) will be stored in the `source` folder. To avoid writing over this file in the following month, You will need to move the PowerPoint files to the appropriate sub folder under `results/presentations/`.
14. Once the files are moved you will need to open the PowerPoint presentation documents to reformat the charts and images. It is helpful to open the previous month's final PowerPoint presentation as a reference for your formatting. 

## Repository Contents

*   `/data`    - Directory and sub-folders of base data for mapping
*   `/results` - Directory and sub folders of final results
*   `/source`  - Source Code Files for the __monthly-crime-reports__ project.
*   `LICENSE`
*   `README`

## Acknowledgements

This automation would not be possible without the [`compstatr`](https://slu-opengis.github.io/compstatr/index.html) package.
[`compstatr`](https://slu-opengis.github.io/compstatr/index.html) was developed by [Christopher Prener, Ph.D.](https://chris-prener.github.io/) & the [SLU Data Science Seminar openGIS Project](https://github.com/slu-openGIS).

## About Washington University Medical Center Redevelopment Corporation

**WUMCRC** is a partnership between **BJC HealthCare** and **Washington University School of Medicine**, working to improve the quality of life for the neighborhoods surrounding the medical campus. In order to achieve this goal in **Forest Park Southeast** and the **Central West End**, **WUMCRC** has invested millions of dollars toward regenerating the market for private investment in businesses and real estate, enhancing human and social service opportunities, and improving the level of physical and personal security.

**WUMCRC** fosters public-private partnerships to strengthen the **Forest Park Southeast** and **Central West End** neighborhoods by facilitating measures to improve security, promoting the development of diverse housing options, enhancing the lives of residents by implementing human and social service initiatives and enriching neighborhoods with infrastructure upgrades and beautification measures. Security, housing, social service provision and physical infrastructure allow for the cultivation of economic development to ensure the long-term vitality of the **Central West End** and **Forest Park Southeast** neighborhoods.
