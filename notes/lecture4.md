# SMPE - Lecture 4 28/10/2021

## Data management

What is research data? Observations collected through experiments, various format, raw or processed.

What is personal data? Data that can be used to identify a person, directly or indirectly.
Some data can redirect to a person if background knowledge is available (ex. MAC address).

What is sensitive personal data? Data that can be used to harm somebody, can lead to discrimination.
It is forbidden to process sensitive data, except with consent or if it is important.
Any process of those data must be declared to authorities.

### Data management plan

Written document that describes how data are acquired, generated or used during a research process
and the mechanisms used during and after the project. FAIR, as open as possible and as closed as necessary.

*Why data managament plan?*

- Time efficiency: without DMP, difficult to make research reproducible later; with DMP spend some time at
the beginning and then it is faster.
- Impact: correlation between sharing data and citation rates.
- Funding: DMP required by funding societies.

DMP needs to be updated over time.

*Relevant aspects of data management:* related to FAIR principle. DMP can be written by hand or using tools.

- Data description and collection or re-use of existing data:
	- describe sources and licences and the new data collected or produced (why not using existing data?)
	- detail kind, format and volume of data
- Documentation and data quality:
	- describe metadata accompanying data (different kind of metadata), detail used standards (should be the
	one of the research community)
	- use controlled vocabularies if relevant
	- explain organization and followed methodology
	- add README file describing how information is captured and recorded
	- explain data quality control
- Storage and backup during the research process:
	- minimum three backups in different location, automatic backups should be used
	- data security and protection of sensitive data, data recoveries strategies and access rights
- Legal and ethical requirements, codes of conduct:
	- responsabilities for data processing and protection
	- data minimization (reduce risks) and privacy by default
	- detail achievement of compliance with GDPR
	- consider possibal ethical issues
- Data sharing and long-term presentation:
	- describe how and when and which and where data will be shared and preserved
	- describe methods or tools needed to access and use data
	- ensure persistent identifier as DOIs
	- choose license to use
- Data management responsabilities and resources:
	- state who is responsible for data management
	- tools to estimate needed resources

Need to adapt to different domains, legislations, funders and local institutions.


## Comments on firstnames homework

- For geographic data, best visualization is using a map
- How this data have been produced? A pointer to the data is provided, it may change, use a checksum to
verify that it is the one file we want
- One must consider the semantic of the data, departments in France evolved over time
- In R, load values for missing values as `NA`s
- Deal with personal name, if there is only a person with a certain firstname it can be identified, more
rare names gathered together
- One must explore the dataset, read the associated documentation and metadata files
- In R, dataframe can be piped to a plotting function
- In the dataset, the same name is present with different accent, leads to duplicates and missing value
- All manipulations should be noted (ex. capitalize all names without accents)
- For intensity of firstnames numbers should be normalize according to total births


## Introduction to data statistics

It is important to analyse the dataset.

- Data production:
	- depends on the intention of who builds data, biais are always introduced (purpose)
	- the followed approach is important (method)
	- a dataset has to be practically produced, characterization and semantic of data (observations)
- Analysis of the set of variables:
	- understand the role of each variable and why it has been chosen
	- important to build good metadata document and define variable properties, identifying response and
	explanatory variables
- Data production:
	- datasets are not building without the need of a decision at the end, it coincides with risks
	- quality of dataset implies quality of decision
- Quality criteria:
	- EUROSTAT: relevance, accuracy, timeliness, comparability, coherence, accessibility
	- Berti-Equille: interpretability, unicity, conformity to norm, consistency
- Pre-processing:
	- look at data before doing any analysis, understand the data
	- there are almost always missing data, try to understand them and give potential explanations
	- state how missing values are treated
