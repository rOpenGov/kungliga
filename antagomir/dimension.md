---
title: "Document dimension preprocessing summary"
author: "Lahti, Marjanen, Roivainen, Tolonen"
date: "2016-06-29"
output: markdown_document
---



## Document size comparisons

  * Some dimension info is provided in the original raw data for altogether 73866 documents (19.1%) but could not be interpreted for 8213 documents (ie. dimension info was successfully estimated for 88.9 % of the documents where this field was not empty).

  * Document size (area) info was obtained in the final preprocessed data for altogether 73551 documents (19%). For the remaining documents, critical dimension information was not available or could not be interpreted: [List of entries where document surface could not be estimated](output.tables/physical_dimension_incomplete.csv)

  * Document gatherings info is originally available for 65653 documents (17%), and further estimated up to 65653 documents (17%) in the final preprocessed data.

  * Document height info is originally available for 7970 documents (2%), and further estimated up to 73551 documents (19%) in the final preprocessed data.

  * Document width info is originally available for 333 documents (0%), and further estimated up to 73551 documents (19%) in the final preprocessed data.


These tables can be used to verify the accuracy of the conversions from the raw data to final estimates:

  * [Dimension conversions from raw data to final estimates](output.tables/conversions_physical_dimension.csv)

  * [Automated tests for dimension conversions](https://github.com/rOpenGov/bibliographica/blob/master/inst/extdata/tests_dimension_polish.csv)



The estimated dimensions are based on the following auxiliary information sheets:

  * [Document dimension abbreviations](https://github.com/rOpenGov/bibliographica/blob/master/inst/extdata/document_size_abbreviations.csv)

  * [Standard sheet size estimates](https://github.com/rOpenGov/bibliographica/blob/master/inst/extdata/sheetsizes.csv)

  * [Document dimension estimates](https://github.com/rOpenGov/bibliographica/blob/master/inst/extdata/documentdimensions.csv) (used when information is partially missing)


  
<!--[Discarded dimension info](output.tables/dimensions_discarded.csv)-->

Left: final gatherings vs. final document dimension (width x height). Right: original gatherings versus original heights where both are available. The point size indicates the number of documents for each case. The red dots indicate the estimated height that is used when only gathering information is available. 


<img src="figure/dimension-summary-1.png" title="plot of chunk summary" alt="plot of chunk summary" width="430px" /><img src="figure/dimension-summary-2.png" title="plot of chunk summary" alt="plot of chunk summary" width="430px" />


Left: Document dimension histogram (surface area). Right: title count per gatherings.

<img src="figure/dimension-sizes-1.png" title="plot of chunk sizes" alt="plot of chunk sizes" width="430px" /><img src="figure/dimension-sizes-2.png" title="plot of chunk sizes" alt="plot of chunk sizes" width="430px" />

### Gatherings timelines




Popularity of different document sizes over time. Left: absolute title counts. Right: relative title counts. Gatherings with less than 15 documents at every decade are excluded:


<img src="figure/dimension-compbyformat-1.png" title="plot of chunk compbyformat" alt="plot of chunk compbyformat" width="430px" /><img src="figure/dimension-compbyformat-2.png" title="plot of chunk compbyformat" alt="plot of chunk compbyformat" width="430px" />



<!--


## Average document dimensions 

Here we use the original data only:

![plot of chunk avedimstime](figure/dimension-avedimstime-1.png)




Only the most frequently occurring gatherings are listed here:


|gatherings.original |mean.width |median.width | mean.height| median.height|  n|
|:-------------------|:----------|:------------|-----------:|-------------:|--:|
|4to                 |NA         |NA           |       23.57|         23.57|  7|
|8vo                 |NA         |NA           |       20.59|         20.59| 32|

-->