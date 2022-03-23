# Detection and categorization of malicious URLs.
SCS 3253 Machine Learning Project | [Website](https://quickheaven.github.io/scs-3253-machine-learning/)

Jupyter Notes:
* [Part I - Import the data and prepare it for modelling](https://github.com/quickheaven/scs-3253-machine-learning/blob/main/Part_I_Import_the_data_and_prepare_it_for_modeling.ipynb)
* [Part II - Train and evaluate the models](https://github.com/quickheaven/scs-3253-machine-learning/blob/main/Part_II_Train_and_evaluate_the_model.ipynb)

Submitted by:
* Arjie Cristobal
* Omair Amjad

## Introduction

### URL dataset (ISCX-URL2016)

The Web has long become a major platform for online criminal activities. URLs are used as the main vehicle in this domain. To counter this issues security community focused its efforts on developing techniques for mostly blacklisting of malicious URLs.

While successful in protecting users from known malicious domains, this approach only solves part of the problem. The new malicious URLs that sprang up all over the web in masses commonly get a head start in this race. Besides that, Alexa ranked, trusted websites may convey compromised fraudulent URLs called defacement URL.

We explore a lightweight approach to detection and categorization of the malicious URLs according to their attack type and show that lexical analysis is effective and efficient for proactive detection of these URLs. We also study the effect of the obfuscation techniques on malicious URLs to figure out the type of obfuscation technique targeted at specific type of malicious URL. We study mainly five different types of URLs:

* **Benign URLs:** Over 35,300 benign URLs were collected from Alexa top websites. The domains have been passed through a Heritrix web crawler to extract the URLs. Around half a million unique URLs are crawled initially and then passed to remove duplicate and domain only URLs. Later the extracted URLs have been checked through Virustotal to filter the benign URLs.

* **Spam URLs:** Around 12,000 spam URLs were collected from the publicly available WEBSPAM-UK2007 dataset.

* **Phishing URLs:** Around 10,000 phishing URLs were taken from OpenPhish which is a repository of active phishing sites.

* **Malware URLs:** More than 11,500 URLs related to malware websites were obtained from DNS-BH which is a project that maintain list of malware sites.

* **Defacement URLs:** More than 45,450 URLs belong to Defacement URL category. They are Alexa ranked trusted websites hosting fraudulent or hidden URL that contains both malicious web pages.

Obfuscation is used as a common method for masking malicious URLs. An attacker intending to evade static analysis on lexical URL features use obfuscation techniques so that malicious URLs become statistically like the benign ones. The obfuscation techniques on URLs is analyzed for the intent of malicious activity in this research. We analyzed mainly Spam, Phishing and Malware URLs to see what kind of obfuscation techniques applied on the URLs.

The full research paper outlining the details of the dataset and its underlying principles:

* Mohammad Saiful Islam Mamun, Mohammad Ahmad Rathore, Arash Habibi Lashkari, Natalia Stakhanova and Ali A. Ghorbani, "Detecting Malicious URLs Using Lexical Analysis", Network and System Security, Springer International Publishing, P467--482, 2016.

Link: [URL dataset (ISCX-URL2016)](https://www.unb.ca/cic/datasets/url-2016.html)

## 1. Required Python libraries

```python

# To plot pretty figures


# Machine learn packages


# Remove all warnings in this notebook
warnings.filterwarnings('ignore')

# Same random seed state
np.random.seed(42)
random_state=42
```

## 2. Load URL dataset

### 2.1 

### 2.2 


## 3. Examine dimensions in a graphic


### 3.1 Split features and targets


### 3.2 


## Choosing my model

### 4.1 Feature Engine


### Machine learning models

Machine learning models:

* k-Nearest Neighbor
* Gradient Boosting
* Random Forest
* Decision Tree
* Logistic Regression
* ADA Boost

## Results


