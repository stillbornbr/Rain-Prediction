# Project Goals
This repository has a end-to-end Data Science project, about climate predictions. It's a particular project that I'm working just myself, to improve my engineering and data analysis-science skills. The main goal is to create a app (In Cloud) that can be access by users that want to know climates predictions.

# Project Description
In resume, this project is split into this parts:
  - Env: Compute Engine / VM Instance - Google Cloud Platform
  - Data Source: API
  - Automation: Python
  - Database: BigQuery
  - IA: Python
  - App: TBD

![image](https://user-images.githubusercontent.com/69798348/115745736-1939a080-a36a-11eb-81f1-cbc88bcb3789.png)

# Documentation

# API:
This API bring the climate info about some region passed in the parameters. For example, if you pass "London", then you receive London Climate info, as Temp, Wind direction, kpm wind, sky condition, etc. The API refresh this info every 15 minutes, thus you have 4 registers per hour about the region you want.

# Starting the project:

At the beggining, we don't have any information about any region climate, so we need to collect and store the data in some database. To solve it, we create a VM Instance in Google Cloud Platform, where we gonna run our scripts and a database in Query, where we gonna store the data. Thus, at this moment, every 15 minutes my scripts runs, collect the data from API, transform and insert into BigQuery table. At some point, we gonna have thousands of registers then we be able to create our predictions models.

# Where we are and what we're doing:
  # 22/04/2021
  This is the first day of collecting data from the API. We're collecting data from a city in Brazil, Carapicuiba, every 15 minute and storing into a BigQuery Table.
  
  # Next days:
  1) Include another cities, as Barueri, Carapicuiba and Sao Paulo, because their next to each other.
  2) Include a automation that sends a signal if the script doesn't finish the job, so we can know if the table has been updated.
  3) Wait for at least 2000 records, then we can create prediction models with this dataset.

# Thanks!
I hope we can update this repository soon!
  
