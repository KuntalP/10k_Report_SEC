# Problem Description
A 10-K FInancial Report is a comprehensive report which must be ﬁled annually by all publicly traded companies about its ﬁnancial performance. These reports are ﬁled to the US Securities Exchange Commission (SEC). This is even more detailed than the annual report of a company. The 10K documents contain information about the Business' operations, risk factors, selected ﬁnancial data, the Management's discussion and analysis (MD&A) and also Financial Statements and supplementary data. 10-K reports are very important for investors and Warren Buffet consistently cites these reports as a great source of information about a company's potential to succeed. 

# About Data
Two datasets are provided to you the '10k_ﬁling_info.csv' ﬁle and the 'ﬁnance_word_dictionary.csv' ﬁle. 
The '10k_ﬁling_info_train_links.csv' has the url to the 10-K ﬁnancial report, identifying information about the company and the target variable. 
The 'ﬁnance_word_dictionary.csv' ﬁle is a dataset from the ‘Loughran McDonald Master Dictionary’. These words are speciﬁcally curated in the context of ﬁnancial reports. You can use the information from this data that you think might be important to vectorize the text extracted from the 10-K reports. 

The '10k_ﬁling_info.csv' ﬁle has the following attributes:

a. Ticker : A symbol with letters identifying the company   

b. CIK : The central Index Key used by the SEC to identify the company  

c. ﬁling_date : The date on which the 10-K report was ﬁled  

d. 10k_link : The link from which the 10-K document has to be scraped   

e. long_term_outlook : The 6 month outlook on the stock price after the date of ﬁling of the report ('0' - Decrease, '1' - Increase)

The link in the dataset gives access to multiple documents. Each document is enclosed inside the <DOCUMENT> and </DOCUMENT> tags Once you extract a document, ensure that you only collect the 10-K report and discard all other documents.

# Approach
A) First we extract the 10k document. This is done in R (Due to the high size of the data, Jupyter Notebook keeps on crashing.)

B) Preprocess the extracted 10k document - train and test

C) Build a classification model without using the dictionary dataset provided.

D) Building a classification model using sentiments extracted from the dictionary dataset.
