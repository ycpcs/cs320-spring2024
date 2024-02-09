---
layout: default
title: "Project: RevMetrix Bowler User Interface"
---

Project Summary
===============
The RevMetrix Bowler User Interface (UI) will allow bowlers to track their performance by providing means for entering their scores, as well as provide access to an array of statistics based on those scores.

Basic Requirements
==================

A bowler participates in several types of **Events**: practice, leagues, tournaments.

The User should be able to register various events through the UI.  Registering an Event includes entering a variety of data related to that Event:

-	**Name:** the name of the Event
-	**Type:** practice, league, tournament
-	**Location(s) of the Event:** the bowling establishment(s) where the Event will occur
-	**Average:** the average for all games thrown for the event
-	**Stats:** the high and low Session scores, high and low game scores from all games for the event, etc...
-	**Sessions:** a list of the Sessions associate with the Event

An **Event** can be composed of one or more Sessions, i.e., a league generally meets weekly at a scheduled time.  Session information will include:
-	**Establishment:** picked from the list for the Event
-	**Date:** date of the Session
-	**Time:** scheduled starting time of the Session
-	**Team Opponent:** for a team Session, the opponent's team name
-	**Individual Opponent:** for match play, the opponent's name (it is possible to have a team opponent and an individual opponent at the same time
-	**Score:** total score for all games in the Session
-	**Stats:** # of first shots, # of strikes, spares, opens, splits, spares converted, splits converted, etc...
-	**Games:** a list of Games associated with the Session

A **Session** consists of a number of Games.  For example, a league Session generally consists of 3 games each week, whereas a practice Ssession could consist of any number of Games (or even partial Ggames - just a series of Fames).  Game information will include:
-	**Lane(s):** the lane(s) on which a Game was bowled.  A Game can be bowled on multiple lanes.  For example, a league Session is generally conducted on an odd-even pair of lanes, alternate Frames between the two lanes.
-	**Game #:** the chronological order of the Game within the Session
-	**Score:** the score for the Game
-	**Starting Lane:** the lane the first Frame was bowled on
-	**Frames:** a list of Frames associated with the Game

A **Game** consists of 10 Frames. Frame information includes:
-	**Frame #:** the chronological order of the Frame within the Game
-	**Lane:** the lane the Frame was bowled on
-	**Result:** indicates the result for the Frame: strike, spare, open, etc...
-	**Shots:** a Frame can have up to three Shots (the first 9 have up to two Shots, the 10th can have up to three Shots

A **Shot** is the most basic component of a Game.  For the first 9 frames, a Frame consists of one or two Shots.  For the 10th Frame, there can be up to three Shots.  The Shot information consists of:
- 	**Shot #:** the chronological order of the Shot within the Frame
-	**Ball:** the Ball used for the Shot
-	**Count:** pins knocked down on the Shot
-	**Leave:**  a list of the number of each pin that was left standing after the Shot
-	**Type:** the type of leave: strike (no pins standing), spare, open, split, washout, etc...


Other Components
================
-	**Account:** an account the User creates in order to enter and interact with their data
-	**Event Registration:** a means for the User to add Events to their Event Collection
-	**Ball Registration:** a means for the User to add Bowling Balls to their Bowling Ball Aresenal (bowling balls that they own/use)
-	**Ball:** an individual entry in the Ball Arsenal
-	**Establishment Registration:** a means for entering a bowling establishment into the collection of bowling establishments that host Events the bowler has/will bowl in.
-	**Establishment:** an individual entry in the Establishments collection



Basic Functionality
===================

## Bowling

-	The bowler will select an Event, Establishment, Session, Lane(s), Bowling Ball(s), and then commence to bowl.
-	The UI will automatically keep track of game, score, lane, ball, frame, and shots.
-	The user will roll each shot, and enter the number of pins left standing using an inverted equilateral triangle of numbered circles	(representing the pin layout at the end of a bowling lane).
-	They will select the pins that were left standing after each shot.
-	The UI will update the count for the shot as the user selects/deselects the pins left standing.
-	The User will be able to select 'X' if they rolled a strike, or '/' if they converted a spare.
-	The User will be able to select 'F' if the fouled, or '-' if they threw a gutterball, or missed all of the pins on a spare.
-	After the User has finished their selection for a shot, they will submit that shot, and the shot information will be sent to the Revmetrix System for analysis, storage, processing, and storage.
-	The System will then respond and set up the next shot, or the next frame, while also displaying the current score and the bowling performance so far in the game, on a fram by-frame basis.
-	The User should be able to select the ball used on shot - and the System should remember which ball was last used so that the User does not have enter the ball for every shot.
-	The User can also specify different bowling balls for 1st and 2nd shots, and for different lanes, and the System will track and display that informatin automatically, as well.

## Statistics

The bowler will be able to retrieve a wide array of statistics from the games that they have bowled.  Those statistics (or "metrix", it is called *RevMetrix* after all) will be represented in both **numeric** and **graphical** form:

-	**League Average**: the average of all games bowled in a league
-	**Game Average:** averages of 1st games, 2nd games, 3rd games bowled in a league
-	**Average Trend:** Graph of average over the entire league, all leagues, all first games over a date range, running sum average for a certain # of games for a given date range, etc...
-	**High and Low Games:** across all Events, across a certain league, across certain 1st, 2nd, 3rd games within a league, etc...
-	**Histograms of Scores:** distribution of 180'2, 190's, 200's, 210's, 220's, etc., for a given Event or date range
-	**Pocket Percentage:** percentage of 1st shot attempts that hit the pocket, percentage of pocket hits that resulted in strikes, etc...
-	**Pocket Quality:** percentage of light pocket hits, high oockets hits, solid pocket hits, and the percentage of each that resulted in strikes, and the types of leaves when not strikes
-	**Strike Percentage:** percentage of first shots that are strikes (across all events, a league, across a date range, for a given ball, etc.)...
-	**Spare Percentage:** similar to above for spare attempts
-	**Leave Percentage:** the percentage of leaves that are 10-pins, all single-pin leaves, splits, etc...
-	**Conversion Percentage:** the percentage of leaves that were converted (# of 10-pins made)
-	**Recent Performance:** a wide variety of other *metrix* for performance on strikes, spares, average, etc...
-	**AND SO MUCH MORE...  :-)**