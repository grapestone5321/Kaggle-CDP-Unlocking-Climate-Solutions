# Kaggle-CDP-Unlocking-Climate-Solutions
Kaggle-CDP-Unlocking-Climate-Solutions

## CDP: Carbon Disclosure Project
https://www.cdp.net/en

### Wikipedia
https://en.wikipedia.org/wiki/Carbon_Disclosure_Project

The CDP (formerly the Carbon Disclosure Project) is an international non-profit organisation based in the United Kingdom, Germany and the United States of America that helps companies and cities disclose their environmental impact. 

It aims to make environmental reporting and risk management a business norm, driving disclosure, insight, and action towards a sustainable economy.

Since 2002 over 8,400 companies have publicly disclosed environmental information through CDP.

## Modelling
### What next?
- Suggested analysis and modelling techniques that you can be apply as you tackle the competitions problem statement.

- Suggestions below are only a guide. You are not limited to these approaches - use your imagination and publically available data to tackle this challenge from any angle you can dream of!

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


## GitHub: Getting started with NLP: Traditional approaches
https://github.com/edumunozsala/Intro-NLP-Text-Classification/blob/master/Intro_NLP_1_TFIDF_Text_Classification.ipynb

