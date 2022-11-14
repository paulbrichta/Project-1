#  <span style="color:tan"> **Module 7 Project**  </span>

## Team 1:  PyWear Disc Golf Apparel


# 🦜 🏴‍☠️ ☠️ 💰 💰 💰 💰 💰 ☠️ 🏴‍☠️ 🦜

Meet the Pyrates:
* Rahma Ali
* Paul Brichta
* Chris Gruenhagen
* Jason McHone

---

#  <span style="color:tan"> Data Preparation Matrix </span>

## <span style="color:tan"> Resources </span>
|	Resource files	|	Contents			|	Source	|
|	---------------------------------------------------------	|	---------------------------------------------------------			|	--------------------------------------------------------------------------------------------------------------------------------------	|
|	DiscGolf.csv	|	Disc Golf course data			|	https://www.kaggle.com/datasets/lanekatris/pdga-united-states-disc-golf-courses	|
|	postcode_level_averages.csv	|	average income by zip code			|	https://www.kaggle.com/datasets/hamishgunasekara/average-income-per-zip-code-usa-2018	|
|	2010_and_2014_county_population_density.csv	|	Population density by county			|	https://odn.data.socrata.com/dataset/2010-and-2014-county-population-density/mmzq-86sd	|
|	Unemployment.csv	|	median household income by county			|	https://www.ers.usda.gov/data-products/county-level-data-sets/	|
|	FIPS_CODES.csv	|	County IDs for choropleth map			|	https://transition.fcc.gov/oet/info/maps/census/fips/fips.txt	|
|	python module geopy.geocoders	|	county names by latitude/longitude			|	Python module geopy.geocoders	|
|	csvData.csv	|	Population density by state			|	https://worldpopulationreview.com/states	|

---
<br>
<br>

## <span style="color:tan"> Data Preparation Jupyter Notebooks</span>

|	Jupyter Notebooks	|	Contents					|
|	---------------------------------------------------------	|	--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------					|
|	P1_data_prep_final.ipynb 	|	primary data preparation notebook					|
|	P1_data_prep_county_final.ipynb	|	supplemental notebook that incorporates the county data into the original dataset.  Data loss of approx 3% during processing.  234 records did not match with county pop density and/or median income records.					|
|	P1_data_prep_Choropleth_final.ipynb	|	supplemental notebook to update the data and create a Minnesota county cloropleth map.  Data loss of approx 2% during reprocessing.  153 records removed at county merge.					|
---
<br>
<br>

## <span style="color:tan"> Data Preparation Output Files</span>

### <span style="color:LightBlue"> P1_data_prep_final.ipynb  output files  </span>
|	File name	|	n rows	|	Comments	|	Contents	|
|	---------------------------------------------------------	|	-------	|	------------------------------------------------	|	--------------------------------------------------------------------------------------------------------------------------------------	|
|	draft_dgolf_avincome.csv	|	6770	|	WIP doc, data exploration	|	original disc golf course info by zip code, no pop density or median income	|
|	draft_dgolf_region.csv	|	6770	|	WIP doc, data exploration	|	original disc golf course info by zip code and region, no pop density or median income	|
|	draft_dgolf_statesummary.csv	|	50	|	for Team analysis use	|	summary of dgolf_region.csv by state (contains Alaska data), no pop density or median income	|
|	draft_dgolf_regionsummary.csv	|	5	|	for Team analysis use	|	summary of dgolf_region.csv by region (contains Alaska data), no pop density or median income	|
|	dgolfdf.csv	|	6770	|	WIP doc	|	copy of dgolfall.csv with an added column "county_clean" to fix Saint vs St. in county names.	|
|	dgolf_county.csv	|	6536	|	WIP doc, data exploration	|	post-merge disc golf course info by zip code and county, with pop density and med income	|
|	dgolf_region.csv	|	6536	|	WIP doc, data exploration	|	post-merge disc golf course info by zip code, county and region, with pop density and med income	|
|	dgolf_summary_area	|	1972	|	For Team analysis use	|	summary of dgolf_region.csv by area (county&state), with pop density and med income	|
|	dgolf_summary_state	|	49	|	For Team analysis use	|	summary of dgolf_region.csv by state with pop density and med income	|
|	dgolf_summary_region	|	5	|	For Team analysis use	|	summary of dgolf_region.csv by region with pop density and med income	|
<br>

### <span style="color:LightBlue"> P1_data_prep_county_final.ipynb output files						
|	File name	|	n rows	|	Comments	|	Contents
|	---------------------------------------------------------	|	-------	|	------------------------------------------------	|	--------------------------------------------------------------------------------------------------------------------------------------
|	CountyIncome.csv	|	3141	|	WIP doc	|	median HH income by county (from Unemployment.csv)
|	CountyPopDensity.csv	|	3140	|	WIP doc	|	population density by county (from 2010_and_2014_county_population_density.csv)
|	dgolfall.csv	|	6770	|	WIP doc	|	add county info to draft_dgolf_avincome data using python module geopy.geocoders
|	dgolfcounty.csv	|	6536	|	WIP doc	|	merge of dgolfall, CountyIncome, and CountyPopDensity data
<br>
### <span style="color:LightBlue"> P1_data_prep_Choropleth_final.ipynb output files	</span>					
|	File name	|	n rows	|	Comments	|	Contents
|	---------------------------------------------------------	|	-------	|	------------------------------------------------	|	--------------------------------------------------------------------------------------------------------------------------------------
|	CountyIncomeCHROMO.csv	|	3141	|	WIP doc	|	median HH income by county (from Unemployment.csv)
|	CountyPopDensityCHROMO.csv	|	3140	|	WIP doc	|	population density by county (from 2010_and_2014_county_population_density.csv)
|	dgolfdfCHROMO.csv	|	6617	|	WIP doc	|	every disc golf course with info by zip code, with pop density and med income
|	dgolfcountyCHROMO.csv	|	6617	|	WIP doc	|	every disc golf course with info by zip code and county, with pop density and med income
|	dgolf_regionCHROMO.csv	|	6617	|	WIP doc	|	every disc golf course with info by zip code, county and region, with pop density and med income
|	dgolf_FIPSmn_CHROMO.csv	|	338	|	WIP doc	|	every MN disc golf course with zip, county, region, fips, with pop density and med income
|	dgolf_FIPSmnmap.csv	|	80	|	For Choropleth analysis	|	Minnesota county summary data for choropleth map
|	MNCounties.png	|	none	|	For presentation	|	MN choropleth map 
|	MNCountiesreverse.png	|	none	|	For presentation	|	MN choropleth map with reverse coloring


