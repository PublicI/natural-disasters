# medicaid-conflicts-analysis
A Center for Public Integrity data analysis for a project investigating the influence pharmaceutical companies exercise over state Medicaid programs' drug purchasing decisions.

Natural disasters might seem like equal-opportunity events. But people with fewer resources and less political power have a harder time recovering after a hit, and they're more likely to die. As climate change worsens extreme weather, the Center for Public Integrity and its partners investigate how government is failing to protect America's most vulnerable residents.



## Data dictionary

NOTE: The definitions for fields pulled from the Federal Emergency Management Agency (FEMA) dataset for this dataset are from their open dataset and are available here. Some have been altered for clarity. The rest are written by the Center for Public Integrity based on U.S. Census Bureau data. More information on the latest census data we analyzed is available here.

*disasternumber: Sequentially assigned number used to designate an event or incident declared as a disaster. 
*ihprogramdeclared: Denotes whether the Individuals and Households program was declared for this disaster. FEMA says to determine which disasters have triggered its Individual Assistance program to use both this field and the individual assistance field, labeled as iaprogramdeclared.
*iaprogramdeclared: Denotes whether the Individual Assistance program was declared for this disaster. FEMA says to determine which disasters have triggered its Individual and Household program to use both this field and the Individual assistance field, labeled as ihprogramdeclared.
*paprogramdeclared: Denotes whether the Public Assistance program was declared for this disaster.
*hmprogramdeclared: Denotes whether the Hazard Mitigation program was declared for this disaster. 
*state: The name or phrase describing the U.S. state, district, or territory.
*declarationdate: Date the disaster was declared.
*fydeclared: The fiscal year the disaster was declared.
*incidenttype: Type of incident such as fire or flood. The incident type will affect the types of assistance available. 
*title: Title for the disaster.
*incidentbegindate: Date the incident itself began.
*incidentenddate: Date the incident itself ended.
*disasterCloseOutDate: Date all financial transactions for all programs are completed.
*placecode: A unique code system FEMA uses internally to recognize locations that takes the numbers “99” + the 3-digit county Federal Information Processing Standards (FIPS) code. There are some declared locations that don’t have recognized FIPS county codes in which case we assigned a unique identifier.
*declaredcountyarea: The name or phrase describing the U.S. county that was included in the declaration.
*lastRefresh: Date the record was last updated in the API data store.
*id: Unique ID assigned to the record.
*state_name: The name or phrase describing the U.S. state, district, or territory.
*state_fips: The FIPS code for the state.
*fips_clean: The full FIPS code for each place. This linked relevant county, independent city and tribal reservations to relevant state FIPS codes. 
*geography: The full name of the area receiving a disaster declaration, eg. Merced County, California.
*total_pop: Total population living in the census area.
*non_white: The number of people of color, including White Hispanic people, in the census area.
*pct_non_white: The percent of non-white individuals out of the census area’s total population.
*under_age_five: The number of individuals under the age of five living in the census area.
*pct_under_age_five: The percent of children under 5 out of the total census area’s population.
*age_65_and_over: The number of people who are 65 and older in the census area.
*pct_age_65_and_over: The percent of individuals 65 and over out of the total census area’s population.
*unemployed_pop: The number of individuals who are unemployed in the census area.
*unemployment_rate: The unemployment rate for that census area.
*med_hh_inc: The median household income for that census area.
*hh_snap: The number of households reliant on the Supplemental Nutrition Assistance Program (SNAP), also known as food stamps, in  that census area.
*pct_hh_snap: The percent of households in the census area reliant on SNAP.
*hh_renter_occupied: The number of households renters occupied the census area.
*pct_hh_renter_occupied: The percent of households lived in by renters in the census area. (See “tenure” census question.)
*fips_us: FIPS code for the U.S. 
*geography_us: The full name for the United States. 
*total_pop_us: The total population of the U.S.
*non_white_us: The number of non-white individuals, including White Hispanic people, living in the United States.
*pct_non_white_us: The percent of individuals who live in the U.S. who aren’t white.
*under_age_5_us: The number of children under 5 in the U.S.
*pct_under_age_5_us: The percent of the U.S. population that is under 5.
*age_65_and_over_us: The number of people 65 or older in the U.S.
*pct_age_65_and_over_us: The percent of the U.S. population that is 65 or older.
*med_hh_inc: The median household income in the U.S.
*hh_snap_us: The number of households in the U.S. reliant on SNAP.
*pct_hh_snap_us: The percent of households in the U.S. reliant on SNAP.
*hh_renter_occupied_us: The number of households in the U.S. that are rented. (See “tenure” census question.)
*pct_hh_renter_occupied_us: The percent of households in the U.S. that are rented.
*unemployed_pop_us: The number of people unemployed in the U.S.
*unemployment_rate_us: The unemployment rate in the U.S.
*elderly_score: If the percent elderly (people 65 and older) in the local census area is larger than the national proportion, the score is one. If not, the score is zero.
*youth_score: If the percent youth (children under age 5) in the local census area is larger than the national proportion, the score is one. If not, the score is zero.
*race_score: If the percent of non-white individuals in the local census area is larger than the national proportion, the score is one. If not, the score is zero.
*unemploy_score: If the unemployment rate in the local census area is higher than the national unemployment rate, the score is one. If not, the score is zero.
*med_hh_inc_score: If the median household income in the local census area is lower than the national median household income, the score is one. If not, the score is zero.
*hh_snap_score: If the percent of households relying on food stamps in the local census area is higher than the national proportion, the score is one. If not, the score is zero.
*hh_renter_score: If the percent of households of renters in the local census area is higher than the national proportion, the score is one. If not, the score is zero.
*total_score: The sum of elderly_score, youth_score, race_score, unemploy_score, med_hh_inc_score, hh_snap_score and hh_renter_score. The lowest possible score is zero. The highest possible score is seven.
*region: The region of the country the census district is in, as determined by the census.



## Code and data for "Medicaid: Under the Influence (LINK TO STORY)," a Center for Public Integrity investigation.

### Here's what's in this repo.
### drug_payments.ipynb
This Jupyter notebook contains code used to analyze drug company payments to doctors sitting on Medicaid Pharmacy and Therapeutics Committees or Drug Utilization Review Boards.

### drug_lobbying.ipynb
This Jupyter notebook contains code used to analyze drug industry lobbying of state legislatures.

### drug_spending.ipynb
This Jupyter notebook contains code used to analyze Medicaid and state budget spending.

### create_open_payments.sql
This SQL script contains code used to create tables for the Open Payments general, research, ownership and deleted data sets.

### create_doctors.sql
This SQL script contains code used to create tables for the Medicaid Pharmacy and Therapeutics Committees or Drug Utilization Review Boards and the NPPES registry data sets.

### create_lobbying.sql
This SQL script contains code used to create a table for the NIMP lobbying data set.

### load_open_payments.sh
This Bash script contains code used to load the Open Payments general, research, ownership and deleted data sets into a PostgreSQL database.

### load_open_payments.sh
This Bash script contains code used to load the Medicaid Pharmacy and Therapeutics Committees or Drug Utilization Review Boards and the NPPES registry data sets into a PostgreSQL database.

### load_open_payments.sh
This Bash script contains code used to load the NIMP lobbying data set into a PostgreSQL database.
