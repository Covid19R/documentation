# Project  Documentation

* Package structure

**Option 1 - long**

|date   | state | country | type | cases|
|-------|-------|---------|------|------|
| 2020-03-01| CA| US| positive| 100|
| 2020-03-01| NY| US| positive| 150|
| 2020-03-01| CA| US| tested| 1000|
| 2020-03-01| NY| US| tested| 1000|
| 2020-03-01| CA| US| recovered| 10|
| 2020-03-01| NY| US| recovered| 10|

**Option 2 - long**
|date       |location   |location_type |location_standardized |location_standardized_type |data_type    | value|
|:----------|:----------|:-------------|:---------------------|:--------------------------|:------------|-----:|
|2020-01-21 |Washington |state         |53                    |fips_code                  |cases_total  |     1|
|2020-01-21 |Washington |state         |53                    |fips_code                  |deaths_total |     0|
|2020-01-22 |Washington |state         |53                    |fips_code                  |cases_total  |     1|
|2020-01-22 |Washington |state         |53                    |fips_code                  |deaths_total |     0|
|2020-01-23 |Washington |state         |53                    |fips_code                  |cases_total  |     1|
|2020-01-23 |Washington |state         |53                    |fips_code                  |deaths_total |     0|


**Option 3 - wide**

|date | state | country| positive | tested | recovered|
|-----|-------|--------|----------|--------|----------|
| 2020-03-01| CA| US| 100|1000| 10|
| 2020-03-01| NY| US| 150|1000| 10|


* Package docs
* Standardized package functions
* Vignettes
* Standardized Vocabulary  
While many of the columns (e.g., location, standardized_location) are variable in their output, the types that are used to describe them are drawn from a standardized vocabulary. Here are the data standards for option 2 - long, with explanation for each.
      - `date`: YYYY-MM-DD
      - `location_type`: Continent, Country, State, Province
      - `location_standardized_type`: fips_code, iso_a3 
      - `data_type`: For temporally dynamic data types, use `*_new` and `*_total` to represent new values for the current day versus cummulative values. cases_new, cases_total, deaths, deaths_total, recovered_new, recovered_total, beds_total, beds_new...

* Data refresh
* Unit tests
* Project contribution
	* Pull request guidance
* Packages usage
