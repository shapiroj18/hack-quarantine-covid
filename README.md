### Hack Quarantine - Covid-19

Website here:
https://hackquarantine.com/

Skillsets:
* James - `Mainly frontend - React/Redux/TypeScript/JS/CSS`
* Mary - `Ruby/Node, graphql/postgresql, has made sinatra microservices, currently tampering in django, very interested in ML/AI`
* Jonathan - `Python/SQL`
* Jerzy - `PHP/Java/Python/JS/Angular`

Timezones;
* James - MST
* Mary - MST
* Jonathan - EST
* Jerzy - GMT

#### Main Idea:
Essentially the key aim of the project is to collect all the covid data on active cases/deaths etc (hopefully classified by underlying conditions or not) to:
a) provide some neat visualisations
b) stick them in an ML model to make some predictions
Rather than a primitive model of projections, I want to see if we can make more accurate projections based on current mitigation strategies (and when they were deployed). We can try to get similar data from comparable countries who are "ahead" in the pandemic. What metrics we use, I don't yet know since I haven't looked at the statistical significance of any data yet. However, I would imagine that factors that may make countries more "similar" will be things like population density, GDP etc.

For example, the UK deployed mitigation strategies later than others... can we build an accurate model based on demographically similar countries that will show what the outcome might have been had we acted sooner. Can we project a worst-case with the government action?


#### Additional Ideas:
* How specific strategies have impacting the curve
* How testing has impacts numbers, provides error etc.
* Looking at the local level
* Tying numbers to demographics (age, gender, ethnicity, etc), population densities, income levels
* How does this disaster compare to other types of disasters? What similar impacts are seen? Thus, what learnings can be gained from best practices in other disaster scenarios? Examples include refugee crises, natural disasters, etc.
* Inaccurate reporting of active cases / Predicting how many active but unreported cases there are (looking at mortality rates) - this was also touched on in the first medium article listed below.
	* It may be possible to estimate unreported cases if we can find some strong enough correlation between cases at 2 separate points in time, then use the exponential curve to figure out what the error is between what should have happened from the past compared to what actually happened with reports. If the newer data point is beyond the first projection then there must have been a large number of unreported cases.
	* You would need people who come in and get diagnosed to report on when they first experienced symptoms, and then keep track of what days they went outside and were possibly exposed to the virus and try to extrapolate from there.
* Worth going through the HackQuarantine doc of ideas as well
* Predict to a granularity of countries since only like US, Italy, China that have decent regional division 
* Blockchain in [medical supply chains](https://www.forbes.com/sites/nishandegnarain/2020/03/22/5-ways-blockchain-can-unblock-the-coronavirus-medical-supply-chain/#21530ebc1380){target = "_blank"}
* BIM (Building Information Modeling) software that could inform hospitals how they can maximize their occupancy, or how to convert other non-traditional venues into pop-up hospitals. Solving for where to put the patients when they run out of hospital beds
	* China was able to build a hospital in \~10 days to support the excess number of patients. Some hospitals/pharmacies are setting things up in parking lots such as fever clinics and drive through testing. 
	* Access city data in hard hit regions in the world and identify where they could potentially set up additional hospital services given that most business have been ordered to remain closed. These could be sports arenas, stadiums, conference centers. Anything that meets the required utilities to help patients. For example, during Hurricane Katrina the state of Louisiana used the SuperDome where the New Orleans Saints play as a shelter for displaced families. 
		* NOTE JONATHAN: use something like GIS with predictive analytics to locate where best to create temporary clinics based on factors?
	* There is a business modeling software that currently exists called [AutoDesk Forge](https://forge.autodesk.com/en/docs/viewer/v2/developers_guide/overview/){target = "_blank"} that we could use that would intake the BIM data and render an image. 
	* Obstacles we may face: Getting that building data from hospitals/venues and learning how to use the software / access the necessary data
* Develop a twitter bot that retweets the tweets of certified experts for each country
	* Twitter API
	* Web Scraping



#### Data Sources (The Johns Hopkins dataset seems to be the go-to for most large-scale data projects):
* WHO
* CDC
* Local newspapers / media networks to understand specific actions taken
* Hospital data
* Google Covid (https://www.google.com/covid19/)
* Kaggle
	* https://www.kaggle.com/c/covid19-global-forecasting-week-1
	* https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge
* https://covid19api.com/
* https://github.com/CSSEGISandData/COVID-19
	* `One of the most cited open COVID-19 datasets is provided by Johns Hopkins University (JHU). Epidemiologists, journalists, and statisticians from around the world are treating this as one of the canonical sources of data on the outbreak. The data is also used to power this interactive dashboard, which tracks reported cases of COVID-19 in real time. As they explain in their article in The Lancet, the Johns Hopkins Center for Systems Science and Engineering developed the dashboard “to provide researchers, public health authorities, and the general public with a user-friendly tool to track the outbreak as it unfolds.”
	The data is pulled in from various sources (primarily DXY), verified by cross-referencing other sources such as the WHO. This dashboard has generally been faster than the WHO in reporting countries’ first cases. The JHU team believes the dashboard is especially useful in providing essential information for appropriate responses in the earliest stages of viral outbreak.[1]`
* https://github.com/beoutbreakprepared/nCoV2019
	* `Another high-quality dataset made available to the public is the nCoV2019 dataset by the Institute for Health Metrics and Evaluation at the University of Washington. The data is presented in this dashboard. The dataset contains highly individual data for each patient such as date of symptom onset, date of laboratory confirmation, and more. It’s intended to aid in calculating key statistics of COVID-19 such as reproduction number, incubation period, and other important factors.[2]`
* https://covidtracking.com/
	* `The most comprehensive data source on US testing and infection rates is the COVID-19 Tracker project.[3,4] The project’s numbers are available on a web page and Google sheet, and via a public API. This project was started in early March, led by a partnership of The Atlantic and the founder of Related Sciences out of concern about the lack of testing information being provided by the CDC. The partners put out a call for volunteers, who quickly developed a collection of software packages to crawl state websites, aggregate the data, and make the dataset available to the public via APIs. The project was developed quickly, and the team shared its source code and datasets. Our World in Data’s page on COVID-19 testing used to list COVID19 Tracker numbers alongside CDC numbers, but now only reports the COVID19 Tracker numbers.`
* https://www.tableau.com/covid-19-coronavirus-data-resources


#### Articles / Visualizations:
* https://medium.com/@tomaspueyo/coronavirus-act-today-or-people-will-die-f4d3d9cd99ca
* https://www.nytimes.com/interactive/2020/us/coronavirus-us-cases.html
* https://www.nytimes.com/interactive/2020/world/coronavirus-maps.html
* https://corona.help/other-stats
* Hack Quarantine resources: https://docs.google.com/document/d/1Y70ObSZCyB308QNbFXelNbl6GAWGfghWA_qJp96awOA/edit
* https://github.blog/2020-03-23-open-collaboration-on-covid-19/ (a wealth of knowledge with good data sources and visualizations)







