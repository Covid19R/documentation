# Project  Documentation

* Package structure
	* Data structure
		* Option 1 - long
		
|date   | state | country | type | cases|
|————-|———————————-|———————————-|————|—————|
| 2020-03-01| CA| US| positive| 100|
| 2020-03-01| NY| US| positive| 150|
| 2020-03-01| CA| US| tested| 1000|
| 2020-03-01| NY| US| tested| 1000|
| 2020-03-01| CA| US| recovered| 10|
| 2020-03-01| NY| US| recovered| 10|
		
		* Option 2 - wide
		
	|date | state | country| positive | tested | recovered|
	|———-|———————————-|———————————|——————-|—————-|————————-|
| 2020-03-01| CA| US| 100|1000| 10|
| 2020-03-01| NY| US| 150|1000| 10|
	* Package docs
	* Vignettes
	* Data refresh
        * Unit tests
* Project contribution
	* Pull request guidance 
* Packages usage
