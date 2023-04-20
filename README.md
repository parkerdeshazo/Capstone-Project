# Super Bowl Winner Prediction using Machine Learning Models

I've been a football fan ever since I can remember. No exaggeration. Some of my very first memories are of me and my dad watching ESPN together on Monday nights to see the
highlights from the weekend. I played for more than 10 years as a kid and I am still a fan today. I haven't found anything that gives me quite the rush that scoring a
touchdown did, but hitting on a three team parlay does feel pretty sweet. And fortunately for me, Louisiana recently legalized sports gambling and is a relatively short
drive away from my hometown of Houston, TX.

Which made me start to think: how cool would it be if I wasn't relying on just my football knowledge and research to make a pick? What if I had something that could
actually look at the data and tell me what's important for a team to win? And what bet would I really be able to leverage something like that on? I did some research and
found that I could consistently get odds somewhere between +600 and +2100 on Super Bowl futures bets, so that seemed like a good place to start.

## The Data

I got all of my data from https://www.pro-football-reference.com/. I looked at historic NFL team statistical data from 2006 to 2022 to determine what makes a Superbowl Winner. I needed to see what the teams with the rings were doing right.
The data included roughly 450,000 data points. It had over 25 different team statistics such passing yards per game, rushing touchdowns per game, defensive interceptions,
and total yards given up in a season.

## Modeling

I used three different models all of which performed similarly in terms of accuracy. First I used a logistic regression model. I knew that the model would struggle with
multicollinearity since a lot of the team stats like offensive touchdown and offensive rank, or defensive turnovers caused and defensive interceptions would correlate strongly
with each other. The model still performed well based on metrics but I was not a fan of it's pick. The Denver Broncos. Next I used a Decision Tree, which picked the New Orleans
Saints. Not a huge fan of that pick either. Finally I used an ADABOOST model which picked the New England Patriots. Not a fan of that pick either but Bill Belichick does
know his way around a Super Bowl. It's also worth noting that ADABOOST also had the Bills coming in second, and that is a team that I personally would feel good about
placing money on.

## Recommendations
After analyzing the features that went in to making a Super Bowl team, there were a few that stood out.
1. Defense: The most important features seemed to be on the defensive side of the ball in general, but having a strong rush defense seemed particularly important.
2. Sling and run the ball: On offense, teams that were able to run the ball well and throw the ball deep were more successful.
3. Take care of the ball: Teams that minimized turnovers were more successful.

## Conclusion
In conclusion, while the models didn't necessarily give me the winning pick, they did provide some valuable insights into what it takes to make a Super Bowl team. 
And let's be real, even if the predictions aren't always accurate, there's nothing quite like the excitement of placing a bet and watching the game unfold. 
So go forth and make your picks, fellow football fans. Just don't blame me if things don't go exactly as planned. As they say, any given Sunday... or Monday... 
or Thursday... or Saturday... you get the point.
