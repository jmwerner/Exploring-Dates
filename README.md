Exploring-Dates
===============

Fun with dates in Julia 
___

###### Motivation

The other day I was wondering what proportion of my life I have lived in California. I suspected it was currently around 10%, but wanted to confirm. More importantly, if I had not reached 10% yet, on what date would I reach 10%? 

###### Usage and Example

Enter your birth date and when you moved to your current location. Next, call the functions `days_since`, `proportion_here`, and `find_day` to find the days since you have moved, the proportion of your life you have spent in your current location, and the day you will reach a given proportion of time in your current location. View the simple example below (executed on 10/29/14) for help with execution.

```
julia> birth_date = Date(2000, 1, 30)
2000-01-30

julia> moving_day = Date(2010, 12, 15)
2010-12-15

julia> days_since(moving_day)
1414 days

julia> proportion_here(moving_day, birth_date)
0.2625324916450056

julia> find_day(.5, moving_day, birth_date)
2021-10-30
```
###### Author's Note
It should be noted that the results could be slightly biased because I did not write the code down to the hour, only the day. Thus, it is possible that in some situations `find_day` could be a day off in either direction and the `proportion_here` could correspondingly be off by a number of hours. 

This code can also be used to find what proportion of your life you have been married or in a relationship. Use this feature at your own risk. 
