# Policing the Pandemic Mapping Project: Data Collection Methodology

### About

The Policing the Pandemic Mapping Project (PPMP) was co-created by ![Alexander McClelland](https://twitter.com/alexmcclelland), Assistant Professor of Criminology at Carleton University, and ![Alex Luscombe](https://twitter.com/alexlusco), PhD student at the Centre for Criminology & Sociolegal Studeies, University of Toronto.

### Referencing

Alexander McClelland; Alex Luscombe, 2020, "Policing the Pandemic: Tracking the Policing of COVID-19 Across Canada", https://doi.org/10.5683/SP2/KNJLWS, Scholars Portal Dataverse, V1, UNF:6:/xIon/9iNdUhSeQblSPQlA== [fileUNF] 

### Data collection
Data on enforcement events is collected using a series of combined approaches: 

- News articles and press releases collected using Google Alerts, a web crawling and notification
service, set to a range of COVID-19/enforcement related keywords; 
- Ongoing web searches of government municipality and police force’s websites and social media accounts;
- Freedom of information requests; and
- Reports from individuals

We understand reports of enforcement from government, including municipalities and police to be the most reliable source of information. While, media reports are less reliable, and when possible, and we work to verify them with other sources, most media reports often rely enforcement numbers already released by police forces or government officials. Verifying a media report can include searching for the origin of reports of enforcement events as reported by enforcement agencies or governments. For example, many enforcement numbers are released by city officials or enforcement agencies via press releases or conferences, or on social media accounts, or websites. The process of verification also happens over time as reports increase, and are reproduced in various media outlets. In some cases, verifying is not possible, as there is only one available media report on an enforcement event.

### Counting "enforcement"
An enforcement event can be a one individual instance of a person receiving a fine for allegedly violating social distancing for example, or it may be a combined number of individual enforcements. For example, individual events are reported in the media, such as when, on April 29, the CBC reported that a Syrian man was ticketed while in a park with his family. This report is input as one enforcement event. Alternatively, the City of Toronto often releases daily information on enforcement of physical distancing and other emergency measures. On June 11, the city indicated: “Bylaw officers issued four tickets in parks.” For us, this report is also included as one enforcement event. 

We count enforcement events from the moment they are reported, even if the event does not reach court, is dropped, stayed, or withdrawn. This is because our project is focused solely on policing and enforcement, and the harms that result. 

Each event appears as one dot on the map, and includes the number of charges, fines issued, and/or individuals involved. 

### Variables
```place```, ```province```, ```lat```, and ```long```: We classify each enforcement event by its location. In general, this will only be the general location of the municipality or jurisdiction that is reported. In some cases, a report will include more specific information, such as with Ottawa, where the local government reported the specific location in the city of each enforcement event that took place. 

```violation```: Based on information in reports, we classify each event in terms of the violation alleged. In some cases, we need to verify reports using other sources to determine the exact violation which led to the enforcement event. where an alleged violation is not reported, we include it in our reports as unspecified. 

```sanction```: description of the alleged violation(s) causing the arrest, charge, and/or fine. Reports sometimes do not include comprehensive information on the actual reason for the arrest, charge, and/or fine. If this information is not available or cannot be verified for accuracy, it remains unspecified.

```fine_certainty```: It sometimes unclear in reports if a person was fined or not. There are three possible values in this variable: yes (certain they were fined), no (certain they were not fined), and maybe (potentially fined, but unclear based on available information).

```number_of_charges_or_violations```: Total number of charges in reports, including those not COVID-related (e.g., if one person was arrested for breaking and entering, drug possession, and coughing on a police officer, the number of charges or violations would be three). 

```number_of_people```: Number of people arrested, charged, and/or fined. When the total number of people is unclear, we indicate the most conservative number (e.g. Gatineau police issued "more than two dozen" tickets, we include 24 tickets in the data set). 

```individual_business```: We classify each enforcement event according to whether they target individuals or businesses. If a report does not specify individual or business, we default to individual. 

```report_month```: In reports, we look for the actual date that the enforcement events took place. In some instances, the exact date is not reported. If that is the case, we use the date of the report of the enforcement event; this is most often the date a media article is published. It should be noted that there is often a time-lag between an actual event taking place and when it is reported to the public. Additionally, when a date range is given for enforcement events, (e.g. 114 tickets were issued between June 14-25, we indicate it as the latest date in our data set. 

```acting_agency```: We classify each enforcement event by the police force or city bylaw authority involved. Due to the complex network of enforcement by city bylaw, municipal, provincial, or federal police forces, in some cases it is not immediately clear. If the exact name of the police force or city bylaw is not included in the enforcement event, we work to verify using other sources to confirm which the police force or city bylaw authority has jurisdiction, and has been granted the power to enforce emergency measures in the region of the event. 

```legislation```: Our tracking includes provincial emergency legislation, such as Ontario’s Emergency Management and Civil Protection Act, provincial public health legislation, such as Québec’s Public Health Act, municipal bylaws, such as the Côte Saint-Luc bylaw mandating face masks, as well as the Federal Criminal Code of Canada, and other Federal laws, such as the Quarantine Act. We classify each event by the specific name of the legislation involved, as well as a general classification for the legislation using the following categories: criminal law, public health law, emergency law, municipal bylaw, and mixed offence. A mixed offence, is and event where more than one legislation category is applied at the same time, this has happened in a number of spitting or coughing events, where the individual is charged under the Criminal Code of Canada, as well as being issued an order under a region’s provincial public health act. Most reports usually indicate the law enabling enforcement that is involved. However, in some cases, if the name of the specific legislation is not included in the report, based on the location of a report we verify the various legislation involved. 

```known_demographic```: Any demographic information included in the available reports.

```event_desc```: A general description of the incident (usually the headline of the media report, press release, or other report).

```event_url``` and ```other_event_url```: Link to main data sources.

### Limitations 
There are a number of limitations to the data we are able to collect, which includes the following: 

- There is a limitation in terms of understanding the total number of individuals based on how enforcement events are reported to the public. For example, when the City of Toronto, on June 11, stated: “Bylaw officers issued four tickets in parks,” we count that as 4 individual people; we are never certain exactly how many people are involved, as it may be the case that one person received multiple tickets. However, based on reviewing hundreds of reports of enforcement events, we have only seen extremely limited instances of individuals receiving multiple tickets at once. 

- Due to the time lag in reporting of events, we may not capture some events until weeks or months after they took place. 

- The sources we rely on are unlikely to capture every incident or enforcement action taken by police and bylaw officers in Canada. What we our data provides are therefore only conservative estimates.
