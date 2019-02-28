# CricketAnalysis
Hi All Welcome

I have done the analysis for the upcoming cricket match between India and Australia which is going to be held in India from 2/3/2019 to 13/3/2019.

There are 6 things which i have predicted

1)Result of each match of the Series
2)Who is going to win the series
3)Who is going to score the highest run
4)Who is going to get highest wicket
5)Who is going to score maximum sixes
6)Who is going to score maximum fours

For prediction i have used two exel files which i have made it manually.
The exel file IndiaStats.xlsx contains all the inforamtion about the players who are playing the above match. All the data are taken from the google
The exel file IndiavsAus.xlsx contain all the inforamtion about all the matches played in India between india and australia.The data here are taken from cricinfo.


For all of the analysis i have followed this sports journel: https://content.iospress.com/articles/journal-of-sports-analytics/jsa196

Please have a look before going through the coding part.

1)Result of each match of the Series: 
First thing which i did is importing the excel file into the workspace.
1)
BA=Runs scored /Innings played−NOI
(2)
BS=Runs scored/ Balls faced
(3)
MRA=100′s+50′s/Innings played
(4)
outrate=number of times batsman got out/number of balls faced by batsman
(5)
BRPI=4*total number of fours+6*total number ofsix′s/Innings played

The Batting Average (BA) given in Equation 1 gives the average runs scored by the batsman in the tournament which considers only the innings played by the batsman and it subtracts it with the number of times batsman was not out during the innings in the tournament (NOI). This is considered because of the assumption that the batsman would have scored more number of runs in case he had a chance of batting. The Batting strike rate (BS) given in Equation 2 provides the information about an average number of runs scored per 100 balls faced by the batsman. To incorporate the consistency of the batsman, we found that Milestone reaching ability (MRA) using the formula given in the Equation 3, which uses the total number of 100’s and 50’s made by the batsman, which contributes to the total score of the team. The aggressiveness of the batsman is measured by the capability of the batsman to hit more number of fours and sixes. To calculate the boundary runs per innings (BRPI) the Equation 5 is used which considers the total number of four’s and six’s hit by the batsman in the tournament.

So i have calculated the value of the above five equation for both the teams.

Then i compared the value of each equation with the other and gave +1 to the team who have a greater value.
Ex- i compared BA of india and BA of Australia , if BA of india is more then +1 is given to india 

In similar way i took into account all of the equation value and assigned values to both the team.

Then i took the aggrigate for both the teams.


After getting the aggrigate of both the team i took into consideration the old records of india vs australia matches from the exel file IndiavsAus.xlsx.


By checking the old records i also assigned vales like if Australia bats for the 2nd innings at Hydrabad it has a greater chance of winning so +1 for that.

Similarly considering various situtation i have provided marks to both the team accordingly.

Addding these marks to the total aggrigate i have found the winnere of the various matches.

According to my analysis India is going to win by 5-0.


2)Who is going to win the series: India is going to win the series.

3)Who is going to score the highest run: For analysing this i have made a new coulmn which contains value of total runs/total innings. 
Then i have sorted them in descnding order. And took the top 5 batsman.
With this i also found the MRA and Outrate for all of them.

Comparing the values it was found that Virat Kohli is going to score the highest runs.

4)Who is going to get highest wicket: For analysing this i have only taken into account the bowlers. And arranged them in descending order on the basic of bowling average. I have also made a new coulmn which contains value of outrate for each bowler.

Taking the above parameter into consideration it was found that Yuzvendra Chahal is going to take the maximum wicket.

5)Who is going to score maximum sixes: For analysing this i have made a new coulmn which contains the value of total no of 6/total no of innings, which gives the value of 6s scored per match by a player. Then i have also taken into consideration BRPI into account.

Taking all the values into account it is found that Rohit Sharma is going to hit the maximum no of 6.

6)Who is going to score maximum fours: For analysing this i have made a new coulmn which contains the value of total no of 4/total no of innings, which gives the value of 4s scored per match by a player. Then i have also taken into consideration BRPI into account.

Taking all the values into account it is found that Shikhar Dhawan is going to hit the maximum no of 4.



The way i followed in of the way for predicting the things, there can be many ways of doing it. 
