# Bancer-rental-intelligence

## About
A rental property intelligence platform that gives renters a detailed overview of the community situation of where they are about to rent that might affect their quality of life while they reside there
### How it works

Crowdsourced data in form of incident reports and general surveys:

We will use incident reports to collect information on things like: Flood propensity, electricity, road conditions, security incidents.

We will use general surveys to collect information on things like: Electricity supply, flood propensity, road conditions, waste management, traffic severity and corresponding peak hours, security situation, water quality and average cost of living.

We will use weather APIs to collect information such as: Air quality, visibility index, precipitation, temperature and humidity.

We will work with past incident report data from reliable GIS dataset, historical traffic data (up to 6 months into the past from current date) and various database to collect following informations: Flood data from GIS databases, traffic data from any reliable traffic dataset or API, electricity supply dataset

Hence we will create the following for data collection:

An incident report form for each incident report
Use a general survey to collect information, using one form for each of these segment (electricity, flood, road, waste, traffic, security, medical, water)
Use API to fetch data for air quality, visibility index, precipitation, temperature and humidity
Use data repositories to get historical data on traffic, past flood occurrences, and past electricity supply.
Data collected with google forms for incident reports and general surveys will be first collected into a google sheet and this google sheet.

API data will be in JSON format

Data from repositories might come in various formats.

Goal is to pipeline all this data into one database such that it is structured correctly and can then be properly analyzed to extract valuable information and insights for renters.
### Data Output

When a location (street, city) is collected: It retrieves information on the location and then it does analysis on that location and presents data to answer the following questions:


#### Electricity:
- Number of hours of power per day
-  Annual electricity outage incident reports with common reasons cited for outage (transformer issues, nationwide issues, cable problems, etc)
- Days with electricity served per week
- General electricity sentiment (Do people believe power is excellent, good, average or poor)
#### Flood Propensity:
- How often it rains
- How likely is it to flood here
- How long does it take for floods to dissipate
- How severe are flood situations
- Access to good drainage system
- General flood sentiment (Do people believe flood propensity is low, medium or rare)
#### Road conditions:
- Type of road (tarred, soil or muddy)
- How common are potholes on the road
- How often does the road flood
- How common are water puddles on the roads
- How accessible is the road to the main road
- General road sentiment (Do people believe road is excellent, good, average or poor)
#### Waste management:
- Is the location serviced by a waste collection company
- Are they occurrences of illegal dumping sites
- How easy is it to dispose of waste
- General waste disposal sentiment (Do people believe waste disposal is excellent, good, average or poor)
- Traffic Severity:
- Traffic severity from city, street to major locations with average duration it takes to and from city, street to each major location, traffic peak hours to and from each of these       major locations:
  - Victoria Island
  - Yaba
  - Ikeja
  - Ajah
  - Epe
  - Orile
  - Badagry
  - Ikorodu
- General traffic sentiment (Do people believe traffic is excellent, good, average or poor)
#### Security situation:
- How likely is a major security indecent in location?
- How close is the nearest first responder location?
- How likely are you to get a response from a first responder?
- Security policy
- Likelihood of police brutality in city, street?
- Likelihood of police extortion in city, street?
- Average Estimated time of arrival of first-responders to city, street in case of an incident.
- General Security sentiment (Do people believe security is excellent, good, average or poor)
#### Medical emergency:
- What is the hospital access like in city, street
- Are there medical first responders in city, street and their estimated time of arrival to city, street.
- How likely are you to get medical treatment from hospital nearby to city, street in an emergency
- General Medical emergency sentiment (Do people believe security is excellent, good, average or poor)
#### Water quality:
- How good is the water supply
- Self-serve or government served water supply access
- Does water need extensive filtration setup for usability
- General water quality sentiment (Do people believe water quality is excellent, good, average or poor)
#### Weather conditions
- Average monthly temperatures, humidity, precipitation, air quality, and visibility
- General Weather sentiment (Do people believe weather is excellent, good, average or poor)
