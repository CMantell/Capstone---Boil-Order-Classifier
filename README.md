# Capstone---Boil-Order-Classifier
### Author: Chris Mantell

## About The Project

This was a capstone project for a Data Science Immersive program at General Assembly and was inspired by Planetary Health Watch, an environmental policy and environmental disease research group.  The goal of this project is to classify boil-orders in the United States using online English news articles with NLP.

#### Importance Of The Project

Potable water is a necessity that should be guaranteed for everyone living in the United States.  However, the Flint Water Crisis (Wikipedia link: https://en.wikipedia.org/wiki/Flint_water_crisis) has shown that this is not the case.  This ongoing and grossly mishandled crisis did not see relief efforts initiated for an extended time due to many reasons.  One of these reasons was the lack of widespread public awareness of the problem.  

Other cities and towns in the United States may also be suffering from non-potable water but these problems may have not come to light due to a lack of public awareness.  In July of 2017, the town of Moore Bend, Missouri had a four year boil-order that finally ended (News article link: http://www.ky3.com/content/news/4-year-long-boil-water-order-finally-ends-437162833.html).  A monitoring system for boil-orders should be developed to inform the public of sites where water quality issues are of concern and to galvanize relief efforts through widespread public awareness.  This boil-order classifier can be used to augment such a surveillance system.

### Project Overview

**Technical Report for a Boil-order Classifier Using Natural Language Processing Techniques on Google News English Articles** explains entire thought process and data science work flow.

The dataset is unlabeled and comes from the HealthMap, an epidemiological and disease surveillance tool that monitors content from many various sources for information on infectious disease outbreaks.  The author of this project was a data curator for this tool and has the required domain understanding of the data.

> 1. Data acquisition, a data dictionary, initial EDA, and web scraping for article text is explained/shown in the notebook titled **Capstone Project - EDA and Web Scraping**.  URLs in the dataset were scrapped and the HTML was saved in multiple batches as .csv's.

> 2. The batches of the web scrapped data were combined and further EDA done in the notebook titled **Combine Soups**.  Text was extracted using NLP and regex functions.  LDA was performed on the resulting text.  LDA topics were validated with the author's domain understanding.  The web scraped text did not pass the validation process.

> 3. LDA was performed on article headlines and the topics were validated with the author's domain understanding.  This passed the validation process and the LDA topics were used to label the data.  Two of the topics were combined and used to build a binary classification model for boil-order alerts.  Model validation was performed with accuracy, precision, recall, and confusion matrix metrics.  This whole process is shown in the notebook titled **Headlines with Word Clouds**.

> 4. Two maps were created with matplotlib of the United States with 2017 data from the original dataset.  One map shows the original data as a single class and one map shows the other with the LDA and author inferred topics.  This is in the notebook titled **Untitled**.

Last edited : 1/5/18

Contact the author with any questions @
chris.mantell@gmail.com

