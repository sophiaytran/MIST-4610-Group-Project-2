# MIST-4610-Group-Project-2

## Team Name
62755 Group 2

## Team Members 
1. Sophia Tran [@sophiaytran] (https://github.com/sophiaytran)
2. Brooke Francis [@bef17821] (https://github.com/bef17821)
3. Pranav Saravanakumar [@Pranav-23-23] (https://github.com/Pranav-23-23)

# Data Set Overview:
## Hate Crime and Bias Dataset:
- Our data set includes hate crime records for every county in New York State, annually, from 2010 through 2022
- It has 823 Rows and 44 Columns
- Data types include String (county and crime type), Int (crime counts),
- The columns include crime type (Crimes Against Persons vs. Property Crimes) and hate-crime bias type 
- The rows group the crime and bias types by year and county 
## Population Dataset:
- To help with deeper analysis, we also added in this population data set
- This data set includes population estimates for every New York county, annually, from 2010 through 2022 and averages them to get one average population over the 12 years 
- It has 16 columns and 62 rows
- Data types include String (county), Int (yearly populations), Decimal (population average)
- We created this data set by compiling data from different excel sheets on the US Census Bureau website
# Limitations in our Dataset:
1. Our original data set did not include any population data, so the first visualizations we made were essentially just population heatmaps and were not very helpful in     comparisons among counties. 
2. The data set also contained 40+ columns, some of which were not helpful for answering descriptive and prescriptive questions. For example, some rows said crime occurred in  “Multiple Counties”, but did not specify specific counties. The amount of information made the data hard to navigate at first. 
3. The original data set did not have any information on Yates county, so this county appears as grey on our visualizations.
# Modifications to our Dataset: 
To address the above limitations, we modified the data by: 
1. We created and added in the population data set. This helped with adjusting the hate-crime counts for population size and allowed us to identify which counties have a higher relative risk rather than just higher totals
2. We divided the columns of the data set into different categories:Race, Religion, Sex, and Gender. We also removed “Multiple Counties” rows. This helped us to organize the data and made it better suited to use for answering our questions.
# Question 1: 
Which counties, relative to population size, are people most likely to experience race, religion, gender, and sex-based hate crimes in New York State?

Why is this important? 
- Looking at how different types of hate crimes vary by county is important because it helps identify where particular groups are at higher risk, supports targeted policy interventions, and allows us to explore how county-level characteristics may be associated with hate crime patterns.
### Race based Hate Crimes per Capita 
<img width="970" height="706" alt="image" src="https://github.com/user-attachments/assets/da3425af-5ce3-4fcd-98e1-3bacc3bab643" />

Overall, this was the most prevalent form of crime that we looked at. 

County with the highest per capita race-based crime: 
- Hamilton County
  ~6.3 per 10,000 people with the lowest population in NY (5,107 as of 2020)

County with the lowest per capita race-based crime:
- Montgomery County
  ~2.2 per 10,000 people, with a population of 49,532 as of 2020 (46 largest county out of 62 in New York)

### Gender-based Hate Crimes per Capita
<img width="970" height="706" alt="image" src="https://github.com/user-attachments/assets/1344a7d4-fa19-47f0-a9e7-b51b1c075e5b" />

County with the highest per capita gender based crime: 
- Cortland County
   ~4.17 crimes per 10,000 people, with a population of 46,809 as of 2020

County with the lowest per capita gender based crime: 
- 30 counties all had 0 hate crimes

We also noted that there is ambuguity in what defines a gender-biased crime which could account for the low rates in some counties. A lot of gender biased crime is classifed as Domestic Violence or various other categories instead of as Gender-biased and therefore wouldn't show up in our data. It is likely that counties that note 0 instances of gender-biased crime do actually have some gender related cases that are categorized differently. 

### Religion-based Hate Crimes per Capita
<img width="970" height="706" alt="image" src="https://github.com/user-attachments/assets/b58f234c-5c73-4d24-8a62-480185dd34d1" />

County with the highest per capita Relgion-based crimes: 
- New York county 
  ~4.4 crimes per 10,000 people. This is the 3rd most populous county in New York. 

County with the lowest per capita religion-based hate crimes:
- Fulton, Genesee, Hamilton, Lewis, Schuyler, Steuben, Wyoming all had 0
- Of the counties that had at least one instance, Chatauqua County had the lease with ~.07701 crimes per 10,000 people. 

Relgion based crimes were the least reported category of crime in our data. We did further research and found that there isn't much variation in religion in mant areas of New york, and the counties that reported no or very few religion-based hate crimes tended to have large populations of people who shared that same religion. Religion is often also less visible than race which could also account for the lower rates. 

### Sexual-Orientation-based Hate Crimes per Capita
<img width="970" height="706" alt="image" src="https://github.com/user-attachments/assets/05e2c0ce-cb84-424a-89e8-1b35a26fcb57" />

Count with the highest sexual orientation based crimes: 
- New York County 
  ~2.23 crimes per 10,000 people
  Also had the most religious hate crimes

Lowest: 15 counties all had 0 hate crimes
- Of the counties that reported crime, Putnam County had the least with ~0.1011 crimes per 10,000 people.

Similarly to religion, sexual orientation isn't always visible which could account for the lower rates of sexual-orientation based crime. 

## Overall Analysis for Question 1: 
- Overall, New York county was the highest in both sexual orientation and religion based hate crimes per capita
This area covers Manhattan and has a population of ~1.65 million
- Race-Based hate crimes were most prevalent overall
- Religion-Based hate crimes and Sexual-Orientation based hate crimes showed similar distribution patterns
- This data could help government’s customize their responses to hate crimes in different regions

# Question 2
Which New York counties show historical trends that suggest future increases in hate crimes, and how should the government allocate resources as a result? Alternatively, what counties suggest little to no change?

Why is this important?
- This question shifts the focus from simply describing patterns to understanding which counties may face growing risks in the future.  By identifying counties with clear upward historical trends, policymakers and leaders can proactively allocate resources, adjust prevention programs, and provide early intervention in areas where hate crimes are escalating. 

### Overall Analysis: 
<img width="1070" height="762" alt="image" src="https://github.com/user-attachments/assets/c114e345-2075-4edf-9074-9dfb5b8b0614" />

This visualization shows hate crime totals over time (2010–2022) for every county in New York State on one combined line chart. 
Each line represents a different county, and the trend lines indicate whether that county’s incidents are generally increasing, decreasing, or steady. 
Because the chart accounts for ALL counties in the state of New York, with the exemption of Yates county, the chart is extremely busy, especially around the lower levels of hate crimes.
This makes the chart visually cluttered and difficult to interpret. We decided to filter our dataset to show only the Top 3 counties with the strongest upward trends and the Bottom 3 counties with the lowest overall hate-crime totals.

### Top 3 and Bottom 3 Analysis: 
Top 3: 

<img width="870" height="726" alt="image" src="https://github.com/user-attachments/assets/fd455af4-d99c-4933-85bd-855827f8a9fc" />

The top three counties with the strongest upward trends were Kings, New York County, and Queens. All three show clear year-over-year increases, along with multiple spikes in recent years. These upward-sloping lines suggest these counties are the most likely to face future increases if current patterns continue.

Bottom 3:

<img width="704" height="778" alt="image" src="https://github.com/user-attachments/assets/9726cbea-925b-4301-9dae-ac047a4f0829" />

The bottom three counties were Lewis, Schuyler, and Wyoming. Their lines are almost completely flat, with counts often at zero or one. There’s no indication of growth or meaningful change over time.

## Question 2 Analysis: 
- Overall statewide trends are highly uneven across counties 
  - The chart showing all counties shows that while many counties stay consistently low, a few counties have clear upward trajectories but the visualization is extremely busy, which confirms that statewide averages hide important local differences
- Kings, New York County, and Queens stand out with sustained increases over time 
  - Our hypothesis for why these counties have experienced multiple recent spikes is that the higher population density in these counties increase the number of interpersonal interactions and likelihood of conflict, which consequently lead to a higher number of hate crime reports
- The bottom 3 counties show almost no incidents across the entire period, and their trend lines are flat. They do not suggest future increases, based on historical behavior.
- This contrast supports a predictive insight and could help allocate resources
  - Instead of forecasting future numbers, the analysis identifies which counties are likely at rising risk based on existing patterns.
 
## Tableau Packaged Workbook 
The packaged workbook containing the visualizations shown above is attached to this repository.
