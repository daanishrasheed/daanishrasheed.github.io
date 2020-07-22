---
layout: post
title: My First Project - Analyzing NBA data
subtitle: Seeing if the pressure of the playoffs impact a player's performance
bigimg: /img/nbalp.jpg
tags: [NBA]
---

The National Basketball Association (NBA) is a professional men’s basketball league in North America, made up of thirty teams(29 within the U.S. and one in Canada). It is considered one of the four major professional sports leagues within the USA and Canada.

The league was founded in New York City on June 6, 1946, as the Basketball Association of America (BAA). It changed its name to the National Basketball Association on August 3, 1949, after merging with the competing National Basketball League(NBL). The NBA’s regular season runs from October to April, with each team playing 82 games. Its playoffs extend into June.

Through a zip file found on the Carnegie Mellon website, which has data on every professional NBA player since 1946, I was able to make inferences on the coherency that an NBA athlete’s performance in the regular season, has with their performance in the postseason (playoffs). Because of many rule changes that have occurred through the years, I am only looking at players that played starting in 1985.

![Chart](/img/chart.JPG){: .center-block :}

The graph above indicates that on average, a player’s performance will decline in every statistical category shown. This could be because of many reasons such that every team that makes the playoffs are ranked in the top half of the NBA, and the teams that meet, will have at least four games to compete with one another. This gives each team a chance to strategize against their opponent and allows them to take their strengths away and expose their weaknesses. This evidently hinders a player’s performance to not be as good as it was in the regular season where there was a random team every day with varying skill levels.

Given these reasons, it would seem like it would be fairer to compare the standard of play of each individual player throughout their career.

![Chart](/img/heatmap.JPG){: .center-block :}

The heat map above clearly shows that in most of the statistical categories, the performance of a player in the regular season has a positive correlation to their performance in the playoffs. However, the field goal % and free throw % do not have a significant correlation probably due to a few outliers. 

The reason why the field goal % has more outliers than the other fields is because every player plays in the regular season but some of those players were rarely ever in the playoffs. For example, if a player only played one game in the playoffs ever, and he took one shot and made it, then his field goal % will be 100% which is realistically impossible to achieve for any consistent player.

To get rid of these outliers, the players who barely have any experience in the playoffs must be filtered out.

![Chart](/img/heatmap1.JPG){: .center-block :}

The heatmap only takes into account players who played at least a hundred playoff games throughout their career meaning they have more experience. Evidently the correlation in every statistic is much stronger than it was in the previous heatmap most notably in FG %.

From these observations, I believe it is safe to assume that the players who perform consistently well in the regular season and at the same time, have more experience in the playoffs, their impact on the court does not change significantly, although their specific stats will decrease.