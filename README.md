# Policing the Pandemic Mapping Project (PPMP) Data Collection Methodology

www.policingthepandemic.ca

### About PPMP

The Policing the Pandemic Mapping Project (PPMP) was co-created by ![Alexander McClelland](https://twitter.com/alexmcclelland), Assistant Professor of Criminology at Carleton University, and ![Alex Luscombe](https://twitter.com/alexlusco), PhD student at the Centre for Criminology & Sociolegal Studies at the University of Toronto.

### Downloading the Dataset

You can download the full dataset from on ![Dataverse](https://doi.org/10.5683/SP2/KNJLWS)

### Citing the Dataset

Alexander McClelland; Alex Luscombe, 2020, "Policing the Pandemic: Tracking the Policing of COVID-19 Across Canada", https://doi.org/10.5683/SP2/KNJLWS, Scholars Portal Dataverse, V1, UNF:6:/xIon/9iNdUhSeQblSPQlA== [fileUNF] 

### Data Collection Methodology
Data on enforcement events is collected using four major approaches: 

- News articles and press releases collected using Google Alerts, a web crawling and notification
service, set to a range of COVID-19/enforcement related keywords; 
- Ongoing web searches of government municipality and police force’s websites and social media accounts;
- Freedom of information requests; and
- Reports from individuals

We understand reports of enforcement from government, including municipalities and police to be the most reliable sources of information. To the degree possible, all reports are verified using other sources. In the case of media articles, verifying information can include searching for the origin of reports of enforcement events as reported by enforcement agencies or governments. The process of verification happens over time as available reports increase.

Rows in the database correspond to "enforcement entries". An enforcement entry includes any instance where COVID-related arrests, charges, and/or fines were reported. As such, a single enforcement entry can include multiple people, over multiple days, facing various sanctions. Enforcement entry are counted from the moment they are reported and verified, even if the event does not reach court, and/or the charges or fines are dropped, stayed, or withdrawn by the acting authority.

### Variables
```place```, ```province```, ```lat```, and ```long```: we classify each enforcement entry by its location. In general, this will only be the general location of the municipality or jurisdiction that is reported. In some cases, a report will include more specific information, such as with Ottawa, where the local government reported the specific location in the city of each enforcement event that took place. 

```violation```: description of the alleged violation(s) causing the arrest, charge, and/or fine. Reports sometimes do not include comprehensive information on the actual reason for the arrest, charge, and/or fine. If this information is not available or cannot be verified for accuracy, it remains unspecified. 

```sanction```: description of the sanction imposed on person/group for the alleged violation(s). If this information is not available or cannot be verified for accuracy, it remains unspecified. 

```fine_certainty```: it is occasionally unclear in available reports if a person was fined or not. There are three possible values in this variable: yes (certain they were fined), no (certain they were not fined), and maybe (potentially fined, but unclear based on available information).

```number_of_charges_or_violations```: the total number of charges in reports, including those non COVID-related. For example, if one person was arrested for breaking and entering, drug possession, and coughing on a police officer (the latter being COVID-related), the number of charges or violations would be three. 

```number_of_people```: the total number of people arrested, charged, and/or fined in a given enforcement entry. When the total number of people is unclear, we indicate the most conservative number. For example, if it were reported that "Gatineau police issued more than two dozen tickets" on a given day, we would count this as 24 tickets. 

```individual_business```: enforcement entries are classified according to whether they target individuals or businesses. If a report does not specify individual or business, we default to individual. 

```report_month```: the month or months the enforcement actions in a given entry took place.

```acting_agency```: the police force or city bylaw authority that carried out the enforcement action(s). 

```legislation```: the law(s) being enforced. This includes provincial emergency legislation, such as Ontario’s Emergency Management and Civil Protection Act, provincial public health legislation, such as Québec’s Public Health Act, municipal bylaws, such as the Côte Saint-Luc bylaw mandating face masks, as well as the Federal Criminal Code of Canada, and other Federal laws, such as the Quarantine Act. 

```known_demographic```: any demographic information included in the available reports.

```event_desc```: description of the incident(s) that took place (usually the headline of the media report, press release, or other report).

```event_url``` and ```other_event_url```: link(s) to the main data sources relied on.
