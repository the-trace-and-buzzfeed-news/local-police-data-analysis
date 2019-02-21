# Analysis of Local Police Data

This repository includes methodologies, data, and code supporting the following articles, published by The Trace and BuzzFeed News:

- "Shoot Someone In A Major US City, And Odds Are You’ll Get Away With It" (January 24, 2019) — [The Trace](https://www.thetrace.org/features/murder-solve-rate-gun-violence-baltimore-shootings) / [BuzzFeed News](https://www.buzzfeednews.com/article/sarahryley/police-unsolved-shootings)
- "5 Things To Know About Cities’ Failure To Arrest Shooters" (January 24, 2019) — [The Trace](https://www.thetrace.org/2019/01/gun-murder-solve-rate-understaffed-police-data-analysis) / [BuzzFeed News](https://www.buzzfeednews.com/article/sarahryley/5-things-to-know-about-cities-failure-to-arrest-shooters)

[*Click here for additional data and code from The Trace and BuzzFeed News's collaboration.*](https://github.com/the-trace-and-buzzfeed-news/introduction)

## Data

The Trace and BuzzFeed News analyzed internal data on homicides, aggravated assaults, and non-fatal shootings from 22 municipal police departments in the United States. You can find a description of the standardization process and the data fields in [this methodology](https://www.documentcloud.org/documents/5692688-Methodology-for-Local-Police-Data.html), and you can download a copy of the [standardized offense dataset](inputs/).

## Data Analysis

The `notebooks/analyze-local-police-data.ipynb` notebook, written in Python, takes the standardized data, and does the following:

- Identifies the main outcome metric (arrest vs. closure) for each agency/offense combination
- Calculates arrest/closure rates, using the main outcomes identified above
- Analyzes Houston's closure rate trends
- Calculates median arrest disparities by offense and victim race
- Calculates agggregate arrest disparities by offense and victim race

Note: To reproduce the findings, you'll need to unzip the `inputs/offenses-standardized.csv.zip` file before running the notebook.

## Data Disclaimer

The data in this repository is a standardization of raw data that police departments provided to The Trace and BuzzFeed News in response to a public records request. We have carefully checked the accuracy of our analysis, and shared our findings with the respective agencies and numerous experts in the law enforcement field prior to publication. We are sharing our data, methodology, and code in order to support further research and reporting on gun violence. However, users of this data may wish to independently verify the accuracy of their findings prior to making them public, as The Trace and Buzzfeed make no representations or warranties as to any third party use of this data.

## Licensing

All code in this repository is available under the [MIT License](https://opensource.org/licenses/MIT). All data files are available under the [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0) license.

## Questions / Comments?

Please contact Jeremy Singer-Vine at jeremy.singer-vine@buzzfeed.com.
