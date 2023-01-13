## Starbucks data
https://www.kaggle.com/datasets/starbucks/store-locations

## Census 
https://data.census.gov/

- Search here for any data at any summary level
- Hierarchy of census geographic entities https://www.census.gov/programs-surveys/geography/guidance/hierarchy.html
- Data available from...

#### Decennial Census 
- Every 10 years
- Entire population
- Limited vars - Race, ethinicty, housing (no age, income)
- Census block summary level

#### American Community Survey
- Annual, aggregated yearly or 5 year chunks
- Sample of population
- Age, sex, income, education, fertility, housing, job-type, etc. (no religion) https://www.bls.gov/lau/acsqa.htm#:~:text=Estimates%20are%20produced%20for%20demographic,status%2C%20disability%20status%2C%20residence%20one
- Summary levels range from census block to state
- List of ACS topics
https://www.census.gov/programs-surveys/acs/guidance/subjects.html

## My census data
- Race: 
  - P1, 2020 Decennial Census, census tract level https://data.census.gov/table?q=p1&g=0100000US$1400000
  - P1, 2020 Decennial Census, county level P1https://data.census.gov/table?q=p1&g=0100000US$0500000
- Hispanic/Latino: 
  - P2, 2020 Decennial Census, census tract level https://data.census.gov/table?q=p2&g=0100000US$1400000
  - P2, 2020 Decennial Census, state level
- Age & Sex: 
  - S0101, 2021 American Community Survey (5 year), census tract level https://data.census.gov/table?q=age&g=0100000US$1400000
  - S0101, 2021 American Community Survey (5 year), county level https://data.census.gov/table?q=age&g=0100000US$0500000&tid=ACSST5Y2021.S0101
- Income:
  - S1901, 2021 American Community Survey (5 year), county level https://data.census.gov/table?q=income&g=0100000US$0500000
- Education:
  - S1501, 2021 American Community Survey (5 year), county level https://data.census.gov/table?q=education&g=0100000US,$0500000&tid=ACSST1Y2021.S1501
- Occupation
  - S2401, 2021 American Community Survey (5 year), county level https://data.census.gov/table?q=occupation&g=0100000US$0500000
- Industry
  - S2403, 2021 American Community Survey (5 year), county level https://data.census.gov/table?q=s2403&g=0100000US$0500000
- Households (building and people)
  - S1101, 2021 American Community Survey (5 year), county level https://data.census.gov/table?q=housing&g=0100000US$0600000&tid=ACSST5Y2021.S1101
- Population Density

There's so many specific data you wouldn't even think of. Take some time later to comb through and see if you can find something interesting

Note: consider getting ACS data at higher summary levels as well, since block-level estimates have large MOE and may not be accurate if aggregated.


## Geographic shape files
For converting lat/long in starbucks data to county, or census tract.
https://www.census.gov/geographies/mapping-files/time-series/geo/carto-boundary-file.html
- Used 2018 county file: cb_2018_us_county_500k.zip

## Census regions
- Map: https://www2.census.gov/geo/pdfs/maps-data/maps/reference/us_regdiv.pdf
- Copy/pasted from here: https://github.com/cphalpert/census-regions/blob/master/us%20census%20bureau%20regions%20and%20divisions.csv 

## Q&A:
How does ACS 5 year aggregation work?  
- Unlike the Census which intends to survey the entire population, ACS only surveys a sample of the population. By using 5 years of surveys, estimates are more precise and can be given at a more granular level. (5 year summaries are available at block level, whereas for 1 year only published for areas with sufficiently large population.) https://www.census.gov/data/developers/data-sets/acs-5year.html

Why use census tract rather than block?  
- The Census data finder doesn't seem to let me bulk export at the block level, and tracts are plenty granular enough.
