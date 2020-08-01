# Why we Choose this Idea

India has largely been Monsoon dependent for its agricultural/drinking water needs and have been blessed with abundant rainfall until recently. A trend observed in the recent years has been increasing dependence of agricultural irrigation on ground water resources. Indian government had spent close to 16,000 crores in the thirty-five years between 1950 and 1985. As a result of this and green revolution, close to 67 percent of irrigation is currently done using groundwater resources.
Central Ground Water Board, responsible for monitoring the ground water resources collects information from 15,640 observation wells as a representation for 30 million ground water resources. This under representation is critical especially since ground water resources typically suffer from a “Out of sight, out of mind” attitude until the bore well runs out one fine day. Not just ground water, drinking water supplied by the corporation suffers from a similar set of issues in most parts of the country. We want to use data and analytics to give the people a sense of the limits of water resource they have access to hence the decision to work on water sustainability.
Our short-term solution is to focus on water consumption, usage, recharge rates, project these data to the end user, and make them cognizant of their water usage. To educate and provide them with a fair idea of their usage and indicate periodically on their usage and how long they can continue with the same kind of usage without running out. The long-term solution involves using these data, anonymize it and to enrich the dataset government works with, to enable better monitoring and reporting of our underwater resources.

## Solution Approach

Our solution aims at providing a detailed view on usage of water in households. Monitoring the hourly usage of water, we are providing insights on their usage and prediction on how far with past trend of usage, the household can sustain with available water. The solution also provides periodic warnings in messages and mails to the house residents to make the water usage more economical. Therefore, with constant monitoring and periodic intimation of water usage, we are aiming to create awareness to public on water utilization and to achieve economic usage of water.

To achieve the above, we have created a prototype by implementing our solution to an individual house. 

IBM Cloud Services used:
1)	IBM Watson IoT 
2)	Node- Red
3)	Cloudant Data base
4)	Cloud Object Storage
5)	IBM Watson Machine Learning
6)	IBM Watson Assistant

Water usage from various IoT sensor devices will be transmitted to IBM cloud and the data is stored in Cloudant database with timestamp. Here we are simulating the data in Watson IoT from Node-Red and uploading to Cloudant database. With this periodic data on water usage, alerts will be send if usage is higher than a pre-defined threshold value. Updating the consolidated usage in another database. We have consolidate the available water recharge in terms of percentage of water usage, water availability is calculated and updated in database on daily basis. ML models are created using IBM Auto AI feature based on seasons (summer, winter, autumn and spring).  Prediction results are obtained based on the previous water utilization data, which in turn will produce a water prediction dashboard to indicate the end user on their usage.
