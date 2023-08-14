# Rubin_Asaf_DA201_Assignment

<h1>Course 2: Data Analytics using Python: NHS data</h1>
  <h3>February 2023</h3>

Grade: 70%
<h2>Context</h2> 
  <p>
The NHS is the publicly funded healthcare system in England. The NHS is incurring significant and potentially avoidable costs from patients missing their appointments, and would like to undertake a data-informed approach to decide how best to handle the problem. The NHS has posed two main questions:

Has there been adequate staff and capacity in the networks?
What was the actual utilisation of resources?

To answer these questions, Python was used to analyse publicly available historical data about appointments at GP surgeries across the country, including national categories, regional appointments and appointment durations. 
</p>

<h2>Analytical Approach</h2>
<p>
Three data files were imported, cleaned and analysed in Python. Each of these three files contains information on the number of appointments in each NHS location from 1 August 2021 to 30 June 2022. 

A descriptive analysis was undertaken to sense check the data and to provide an overarching view of the underlying patterns, trends and spread of the data. More specifically, to understand the number of rows and columns in each file, and the data types of each column.

An initial descriptive analysis of the data revealed the following:
<ul>
<li>There are a total of 106 locations, with six locations tied in first place for the highest number of records (1484). </li>
<li>There are five types of service setting, which in order of frequency are General Practice, Primary Care Network, Extended Access Provision, Other and ‘Unmapped’. </li>
<li>There are 18 types of ‘national categories, of which the most frequent is ‘Inconsistent Mapping’.</li>
<li>There are three appointment statuses, listed in order of frequency: Attended, Unknown and DNA (Did Not Attend). </li>
<li>November 2011 was the month with the highest number of appointments across all locations. </li>
<li>On average, there are 74308 appointments, per month. </li>
  </ul>
</p>

  ![image](https://github.com/AsafRubin00/LSE-Data-Analytics-Using-Python-NHS-data/assets/115939423/8b4bdeaf-8d25-40ff-9969-e1a5ac98c04e)

  Further analysis was then undertaken to arrive at three key findings:
<ol>
<li><b>Unmapped appointments</b>: There are a high number of ‘Unmapped’ appointments, across different service settings and context types. A national category called ‘Inconsistent Mapping’ also appears to occur at a high frequency. </li>
<li><b>Seasonality</b>: The number of monthly appointments peaked in September to November 2021, with subsequent, but smaller peaks in March and May the following year. Further subcategorizing these time periods into seasons (Summer, Autumn, Winter and Spring) shows that General Practice is by far the most common appointment type across all seasons, but the occurrence of ‘Unmapped’ appointments peaks in Summer and Autumn, suggesting that the busiest months have a higher occurrence of unmapped appointments.  </li>
<li><b>Capacity utilisation</b>: Resource utilisation (number of appointments/30 days per month) mirrors the trend of ‘business’ in each month/season, but exceeds 100% in October and November. This suggests that additional resources are needed in these months. </li>
</ol>
</p>
  <h2>Visualisation and Insights</h2>

Data was aggregated and visualized on a monthly, seasonal and aggregate basis to identify underlying trends that may be of use to the NHS. Line plots were used to visualise trends over time. This was done three times, as outlined below.  

First, an analysis of the actual utilisation of resources was undertaken to try answer the question if the NHS should consider increasing staff levels. Appointments from August 2021 to June 2022 shows a trend line that peaks from September to November, then declines until two successive smaller peaks in March and May, respectively. Resource utilisation (number of appointments/30 days per month) shows a similar trendline, but exceeds 100% utilisation in October and November, suggesting that increasing staff levels may help alleviate some of the issues the NHS currently faces.

![image](https://github.com/AsafRubin00/LSE-Data-Analytics-Using-Python-NHS-data/assets/115939423/d5666733-85cc-40ff-a0a0-1e623cce5765)
![image](https://github.com/AsafRubin00/LSE-Data-Analytics-Using-Python-NHS-data/assets/115939423/4bc59f79-1917-451f-8171-854300038f41)

Second, data was considered on a monthly basis by looking at the sum of appointments per month and plotting these on line plots to identify trends in service settings, context types and national categories, over time. Of most interest is the occurrence of ‘Unmapped’ appointments. Unmapped service settings occur at a frequent but consistent level. Unmapped Context Types peak in the busier month of August to November, then decline. There are unmapped and inconsistent mapping national categories, both of which occur relatively consistently throughout the year. 

![image](https://github.com/AsafRubin00/LSE-Data-Analytics-Using-Python-NHS-data/assets/115939423/0e41aaba-b879-41a6-acf6-0be98b0917b7)

Finally, data was considered on a seasonal basis (summer, autumn, winter and spring). All seasons  follow a similar trend. GP appointments are most common. Unmapped appointments are slightly higher than others in Summer and Autumn, but then dip in the winter and spring – mirroring the results of the previous analysis. 

In summary, the results of the visualisation process suggest three key findings:

The high number of ‘unmapped’ appointments and occurrence of inconsistent mapping’ suggests there are insufficient data capturing capabilities and the administrative process requires improvement.
The occurrence of unmapped appointments during the ‘busy’ months suggests a possible seasonality, which can be addressed by resource reallocation. 
Given that demand exceeds capacity in October and November, the NHS seems to have a resource capacity problem during the busiest months. 

  <h2>Patterns and predictions</h2>
Before making any recommendations, it is noted that correlation does not imply causality. The results of this analysis are not intended to directly diagnose the cause of the problem, but to make inferences as to where certain problem areas may lie. Based on the available evidence, three key recommendations are made: 
<br>
<br>
<ol>
<li><b>Improve administration</b>: The NHS should  consider investing resources in its administrative capabilities and to ensure staff is sufficiently trained to capture important details (i.e. appointment types, reasons for cancellations, etc.), especially during busy months. </li>
<li><b>Plan ahead</b>: significant fluctuations in the number of appointments in certain seasons suggests that bottlenecks may be resolved by reallocating resources with a ‘Just-in-time’ approach, where they are needed, rather than being concentrated in certain locations.</li>
<li><b>Increase the number of staff</b>: The NHS consider increasing staff (GP) levels to meet demand, or if possible, to reallocate other qualified professionals to cover GP appointments during the busiest months. </li>
</ol><br>
In addition to these recommendations, it is also suggested that further research should be undertaken to understand the nature of unmapped appointments – what they are, why they happened and why they tend to peak around the busiest months of the year.
