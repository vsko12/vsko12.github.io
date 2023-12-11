---
title: "Assignment 3 - Spatial Data"
categories:
  - Blog
tags:
  - spatial
  - data
  - analysis
---

In an era where digital streaming and social media dominate our media consumption, it's easy to overlook the roots of broadcast media that laid the foundation for today's entertainment landscape. Our journey takes us back to 1962, a pivotal year in the history of radio and television, where the airwaves were the primary source of information and entertainment. For our third assignment, we chose the "Radio and Television Annual Year Book (1962)" to explore and visualize the geographical and economic landscape of this influential era.

### Step 1: Choice of source
We decided to focus particularly on pages 39-41 which contain the lists detailing the "50 Leading National Spot Radio Markets" and "50 Leading National Spot Television Markets" for the fiscal year 1961. Each list includes statistics about the number of reporting stations in that market, and the total time sales (amount of money that was made from selling advertising spots) from national and regional advertisers and sponsors.

![Television Data](/assets/images/tv-1.png)

![Radio Data](/assets/images/radio-1.png)

We assume that this kind of information would have been used by advertisers and broadcasters to understand the market reach and advertising value of radio and television stations across different metropolitan areas in the United States during that time.

### Step 2: Modeling the data. Identifying what data is available from the source

During the process of modeling the data we identified specific data available in the source that pertains to spatial and quantitative elements. Our data included the following components

- Rank based on sales (quantitative component)
- City and State (spatial component)
- Number of Stations Reporting (quantitative component)
- Time Sales figures (quantitative component)

The next task was to extract these data points from the source material. Since the Year Book had already undergone optical character recognition (OCR), the text could be converted into a digital format that could be manipulated. We created a spreadsheet with columns representing each data aspect and manually filled it.

- **Column 1:** Rank
- **Column 2:** City
- **Column 3:** State
- **Column 4:** Number of Stations Reporting
- **Column 5:** Time Sales

### Step 3: Enriching the data and Geocoding

Working further on the spatial component of the data, we improved the structured dataset extracted from the "Radio and Television Annual Year Book (1962)" by adding geocoded coordinates and relevant historical context to each radio and television market. This involved using geocoding services to translate the market cities into precise latitude and longitude coordinates, which allowed for accurate mapping.

The spreadsheet with columns representing each data aspect for television broadcasting is shown below.

![Television Spreadsheet](/assets/images/tv-2.png)

The spreadsheet with columns representing each data aspect for radio broadcasting is shown below.

![Radio Spreadsheet](/assets/images/radio-2.png)

### Step 4: Visualizing the data. Discussion and Interpretation

After geocoding and adding contextual metadata to our dataset, we used [*Kepler*](https://kepler.gl/), a visualization tool that provides mapping capabilities to create a map that spatially represents the data. We mapped the geographic coordinates of each radio and television market.

#### Results
The visual representation of the data from Kepler enabled us to identify patterns, trends, and anomalies within the data. 

The points on the map are color-coded to represent different levels of sales, with darker colors (closer to red) indicating higher sales and lighter colors (closer to white) indicating lower sales.

##### Television Broadcasting
![Television Results](/assets/images/tv-3.png)

The darker red points suggest areas with the highest sales that correspond to be major cities or areas with higher population density. We hypothesized that this could correlate to a greater number of stations reporting and thus more sales. However, we saw that some regions with high number of stations reporting in fact had lesser sales than some other areas with lower number of stations reporting. In particular, the East Coast of the United States shows some of the darkest points.

The points that are colored a lighter red or orange represent areas with moderate sales. These correspond to the smaller cities and typically also had fewer stations reporting. The map shows several of these across the United States, indicating a spread of moderate sales in various regions.

The lightest points, closer to white, represent areas with the lowest sales. These are mostly areas with the least population density, such as rural areas or smaller towns. The map indicates these areas are more scattered, with no significant cluster, suggesting that lower sales figures are widespread but not concentrated in any one region.

The distribution of sales across the map seems to follow population patterns, with higher sales in densely populated areas and along the coasts, particularly the Northeastern United States. The central part of the country shows a mix of moderate to low sales, which mostly reflects the lower population density.

##### Radio Broadcasting
![Radio Results](/assets/images/radio-3.png)

The areas with the highest sales are primarily concentrated in larger metropolitan areas. This is consistent with what we expected, as larger cities typically have more listeners and therefore more potential for higher sales in radio broadcasting.

Areas with points that are a lighter red or orange represent regions with moderate sales. They are again scattered across the country, which suggests that while these areas have a decent amount of sales, they don't match the commercial activity of the largest urban centers.

The points that are very light, close to white, signify areas with the least sales. These correspond to smaller cities or regions with lower population densities. The spread of these points is quite even, indicating that lower sales figures are common across various parts of the country.

Once again, the East Coast shows a significant amount of dark red points, especially around New York, which is expected due to its population and commercial density. Similarly, the West Coast, particularly California, shows high sales in Los Angeles and San Francisco-Oakland areas.

In the Midwest and the South, there's a mix of sales performance, with some areas showing moderate sales (light red to orange points) and others showing lower sales (points closer to white).

##### Comparison of Television and Radio broadcasting sales
Both television and radio broadcasts seem to have the highest sales in major metropolitan areas, as expected. Cities like New York, Los Angeles, Chicago, and Philadelphia show dark points on both maps, indicating high sales in both industries.

The overall geographical distribution pattern is similar for both television and radio, with coastal areas and major urban centers showing higher sales. There are, however, differences in the intensity of sales between television and radio broadcasts. This could be due to differences in market penetration, the number of stations, advertising revenue, and audience size.

For both television and radio, the Midwest and rural areas might show lighter points, indicating lower sales, which could be related to lower population densities.

The regional differences that are specific to either radio or television may be influenced by several different factors such as local preferences, the presence of strong local stations, or regional advertising spending.

For businesses in the television and radio broadcast industry, this visualization could have been instrumental in targeting advertising campaigns, allocating resources, and strategizing market penetration. It shows where the market is strongest and where there might be potential for growth.


