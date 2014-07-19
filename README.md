DevelopingDataProducts
======================

Repo for Data Science Course Developing Data Products

application: 
server.R and ui.R (shiny)

presentation: 
Rpresentation.Rpres (Rstudio Presenter)
Rpresentation.html with image sshot.png  	


#How to crack a combination lock? 
#========================================================
#Project for Coursera's Developing Data Products course  

#What is a Combination Lock?
#========================================================

#The sequence of numbers, symbols or letters on combination locks may be entered using a single rotating dial which interacts with several discs 
#by using a set of several rotating discs with inscribed numerals which directly interact with the locking mechanism.

#Types range from inexpensive three-digit luggage locks to high-security safes. 

#Unlike a regular padlock, combination locks do not use keys.

#For details on different combination locks pls see http://en.wikipedia.org/wiki/Combination_lock. 

#How to crack a combination lock? 
#========================================================

#You have to try in the worst case all possible combinations of the combination lock.
#The mathematical theory for these permutations with repetitions can be found on http://www.mathsisfun.com/combinatorics/combinations-permutations.html.

#An easy number (10 numbers: 0 to 9) combination lock with 3 rings has  
#```{r}
#10^3
#```
#1000 combinations which was calculated with an R formula.


#Detailed Program Description
#========================================================
#This slide explains how the number of combinations of a combination lock are calculated with as a Shiny application.
#- The application consists of two parts: server.R and ui.R
#- server.R creates a server instance which takes two values (the number of symbols on the rotating dial and the number of discs) , computes the number of possible permutations and returns the result 
#- ui.R creates the html code for a sidepanel containing two text fields that only take numeric values between 1 and 20. 
#- A button within ui.R triggers server.R to calculate the number of combinations.
#- ui.R displays the result returned by server.R in the main panel next to the input fields