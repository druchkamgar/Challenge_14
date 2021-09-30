# Challenge_14
## Purpose 
To create a trading algorithm and backtest it. The trading algorithm produces trading signals by using a short and long simple moving average (SMA). When the two SMAs intersect a trade signal is produced. Namely, when the short SMA rises above the long SMA a buy signal is produced, and vice versa.


## Results
We first trained the algo over a three month window from 2015-08-12 13:15:00 to 2015-11-12 13:15:00 and ran the strategy from 2015-11-12 13:15:00 until 2021-01-22 15:45:00. We used a short SMA of 4 days and a long SMA of 100 days. Under these conditions, the strategy returned ~1.5. 

We next increased the training window to 4 months and reran the strategy. This reduced performance from 1.5 to 1.4. When we reduced the training window to 2 months, the impact to performance on the test data set was similar.

We next adjusted the short SMA. First we increased the short SMA from 4 days to 10 days. This reduced performance from 1.5 to 1.0. We next reduced the short SMA from 4 days to 2 days. This increased performance from 1.5 to 1.6.

The optimal results occured when we used a three month training window and a short SMA of 2 days. See plot below:

![/Users/Dariush/Desktop/Columbia_Challenges/Challenge_14/Screen Shot 2021-09-30 at 11.02.05 AM](/Users/Dariush/Desktop/Columbia_Challenges/Challenge_14/Screen Shot 2021-09-30 at 11.02.05 AM.png)