# Big moves on Mondays
The strategy suggests that we go long on the S&P 500 on a Monday and close our position on the friday that week on certain conditions. 
We assume that positions can be taken only in periods when markets are open from Monday to Friday in a week and the friday in the previous week.

We calculate the following indicators and backtest the conditions shown below:

1. Calculate the 25 day average of relative_range = (High - Low) / Close and call it rel_range_ma.
2. The Monday Close must be lower that the previous Friday the previous Friday Close by at least 0.25 times of rel_range_ma.
3. Create a variable ibs = (Close - Low)/(High - Low). It must be lower than 0.3.
4. If conditions in 2, and 3 are met, go long on monday Close.
5. Square off your position on Friday Close.nday
