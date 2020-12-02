# Kaggle-CDP-Unlocking-Climate-Solutions
Kaggle-CDP-Unlocking-Climate-Solutions

### End Date (Final Submission Deadline): 
12/02/2020 11:59 PM UTC

### Winners announced:
12/16/2020

-------

## Submission
### CDP-Unlocking Climate Solutions: 8. Energy
https://www.kaggle.com/grapestone5321/cdp-unlocking-climate-solutions-8-energy

-------


## CDP: Carbon Disclosure Project
https://www.cdp.net/en

### Wikipedia
https://en.wikipedia.org/wiki/Carbon_Disclosure_Project

The CDP (formerly the Carbon Disclosure Project) is an international non-profit organisation based in the United Kingdom, Germany and the United States of America that helps companies and cities disclose their environmental impact. 

It aims to make environmental reporting and risk management a business norm, driving disclosure, insight, and action towards a sustainable economy.

Since 2002 over 8,400 companies have publicly disclosed environmental information through CDP.

-------

### PROBLEM STATEMENT

- Develop a methodology for calculating key performance indicators (KPIs) that relate to the environmental and social issues that are discussed in the CDP survey data. 

- Leverage external data sources and thoroughly discuss the intersection between environmental issues and social issues. 

- Mine information to create automated insight generation demonstrating whether city and corporate ambitions take these factors into account.

-------

## Evaluation
### HOW TO PARTICIPATE
To make a submission, complete the submission form. 

Only one submission will be judged per participant, so if you make multiple submissions we will only review the most recent entry. 

A starter notebook demonstrates how to load and work with the data.

To be valid, a submission must be contained in one or more notebook, and made public on or before the submission deadline. 

Participants are free to use any datasets in addition to the official Kaggle dataset, but those datasets must be public and hosted on Kaggle for the submission to be valid.

### SUBMISSIONS WILL BE EVALUATED ON THE FOLLOWING
### Accuracy/Completeness

- Did the author develop one or more key performance indicators (KPIs)?

- Did the author provide a way of assessing the performance and accuracy of their solution?

- Are the KPIs useful for discussing relationships between social issues and environmental issues and demonstrating whether city and corporate ambitions take these factors into account?

- Do the KPIs accurately reflect the underlying data?

### Communication

- Does the notebook have a compelling and coherent narrative?

- Does the notebook contain data visualizations that help to communicate the author’s main points?

- Did the author include a thorough discussion on the intersection between environmental issues and social issues?

- Was there discussion of automated insight generation, demonstrating whether city and corporate ambitions take these factors into account?

### Documentation

- Is the code documented in a way that makes it easy to understand and reproduce?

- Were all external sources of data made public and cited appropriately?

-------

## Overview of the Data:
The CDP dataset consists of publicly available responses to 3 different surveys: 

(1) corporate climate change disclosures; 

(2) corporate water security disclosures; and 

(3) disclosures from cities. Data is available for 2018, 2019, and 2020, along with a small collection of supplementary datasets. 

A starter notebook demonstrates how to load and work with the data.

-------



## CDP Competition Starter Notebook

https://www.kaggle.com/callumr22/cdp-starter-notebook

Example data mapping, EDA and data wrangling pipeline to relate CDP Corporate response data to CDP Cities data and external data sets containing social equity data.

### Parameters

### Input
### CDP Corporate Questionnaire response data sets

- 2019_Full_Climate_Change_Dataset.csv = 2019 Climate Change publically disclosed questionnaire responses for North America

- 2019_Full_Water_Security_Dataset.csv = 2019 Water Security publically disclosed questionnaire responses for North America

### CDP Cities Questionnaire response data sets

- 2020_-_Full_Cities_Dataset.csv = Full 2020 Cities Questionnaire response data set

### CDP Cities Meta data sets

- NA_HQ_public_data.csv = CDP curated Organisations metadata, mapping publically disclosed North American organisations to HQ city and state

### External Non-CDP data sets

- SVI2018_US.csv = US Centers for Disease Control and Prevention (CDC) Social Vulnerability Index (SVI) Data for 2018 (Census tract level) - available publicly at

https://www.atsdr.cdc.gov/placeandhealth/svi/data_documentation_download.html

- SVI2018_US_COUNTY.csv = US Centers for Disease Control and Prevention (CDC) Social Vulnerability Index (SVI) Data for 2018 (County level) - available publicly at 

https://www.atsdr.cdc.gov/placeandhealth/svi/data_documentation_download.html

- uscities.csv = metadata for United States cities and towns, with information such as populations size, median age and lat,lng location coordinates - available publicly at

https://simplemaps.com/data/us-cities.

SVI 2018 Documentation and Data Dictionary https://www.atsdr.cdc.gov/placeandhealth/svi/documentation/SVI_documentation_2018.html

### Output
EDA and Visualisations to begin investigating the CDP competition data sets, environmental performance indicators and social-equity KPIs.


## Modelling
### What next?
- Suggested analysis and modelling techniques that you can be apply as you tackle the competitions problem statement.

- Suggestions below are only a guide. 

You are not limited to these approaches - use your imagination and publically available data to tackle this challenge from any angle you can dream of!

### NLP principles to investigate the social-environmental overlap between Corporations and Cities Climate Change 'Readiness'

- Utilise pythons NLP capabilities and tokenization approaches such as Term Frequency–inverse Document Frequency (TF-IDF) (1) to construct a Document Term Matrix (DTM) from questionnaire responses, highlighting key terms in free text answers to aid in topic identification

    - e.g. summarise city 'readiness' for climate change and the hazards they anticipate (Cities Question 2.1)
    - e.g outline the future adaptations cities must implement to prepare for environmental challenges (City Question 3.0)
    - e.g. find common topics in examples of colloboration between cities and business on sustainability projects (City Question 6.2a)

- Apply sentiment analysis to detect whether a city sees opportunity (positive sentiment/polarity) (Cities Question 6.0) or concern (negative sentiment/polarity) (City Question 2.2) over future climate scenarios

- Combine DTM and Sentiment analysis to build a combined KPI that incorporates measures of sentiment and susceptibility into one metric, identifying cities with high levels of percieved risk who may be open to colloboration with business as they foster climate resilience.

    - e.g. Sentiment x Susceptibility  = Climate Risk Sensitivity Score

### Social Accounting with Water Shadow Price Modeling

Using external datasets and water-related risks identified by Corporations (Water Security Question W4.2), build a 'Shadow Price' of water for Corporations operating in a selection of North American cities.

- A shadow price (3) can attempt to account for the total cost of a Corporations water use, estimating all internal and external costs ,as well as exposure to water stress.

- The shadow price coefficient can be combined within volumetric withdrawal data (Water Security Question W5.1a) to assign a Water Risk Cost per company, weighting corporate activties with a measure of the inersection between environmental risks and social impact.

    e.g. Water risk cost for Company = Shadow price for Company * Water withdrawal volume for Company


### References

- Muñoz (2020). Getting started with NLP: Tokenization, Document-Term Matrix, TF-IDF. Medium. 

https://medium.com/analytics-vidhya/getting-started-with-nlp-tokenization-document-term-matrix-tf-idf-2ea7d01f1942

- Reyes-Menendez A, Saura JR, Alvarez-Alonso C. Understanding #WorldEnvironmentDay User Opinions in Twitter: A Topic-Based Sentiment Analysis Approach. Int J Environ Res Public Health. 2018;15(11):2537. Published 2018 Nov 13. doi:10.3390/ijerph15112537. 

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6267440/

- FIR-PRI. Portfolio Analysis Using Water Shadow Pricing: How Valuing Water Risk Can Reduce Carbon Emissions. 

https://www.fir-pri-awards.org/wp-content/uploads/MasterThesis_Chisem.pdf

-------

## GitHub: Getting started with NLP: Traditional approaches
https://github.com/edumunozsala/Intro-NLP-Text-Classification/blob/master/Intro_NLP_1_TFIDF_Text_Classification.ipynb

