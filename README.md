# Degrees Of Separation
This is an AI algorithm written in Python that uses BFS to find the degree of separation between two actors. This is a project for the Harvard CS50 AI Python course.
For example, if actor A stars with actor B in a movie, and B stars with C in another movie, A and C are 2 degrees of separation apart.

The following files can be edited, although there are already some examples already within the files to demonstrate:

# /large/movies.csv

DO NOT edit or remove the first line

for each movie you would like added to the game, input the movie ID (found in the URL of the movie's IMDB page), the title in quotation marks, and the year the movie released
    
example:
      
  	3783958,"La La Land",2016
    2582802,"Whiplash",2014
    
# /large/people.csv

DO NOT edit or remove the first line
 
 for each person you would like added to the game, input their user ID (found on the url of the actor's IMDB page), the person's name, and the year of birth
 
example:

	0799777,"J.K. Simmons",1955
  	0331516,"Ryan Gosling",1980
  	1886602,"Miles Teller",1987

# /large/stars.csv     
   
DO NOT edit or remove the first line

input some person's ID from /large/people.csv, followed by the movie ID of a movie this person stars in.
    
  In this example, we take Ryan Gosling (ID: 0331516) and assign him to the movie "La La Land" (ID: 3783958)  
  Then J.K. Simmons (0799777) to "La La Land" (3783958)  
  Then J.K. Simmons (0799777) to "Whiplash" (2582802)  
  Then Miles Teller (1886602) to "Whiplash" (2582802)

example:
     
	0331516,3783958
  	0799777,2582802
    1886602,2582802

After inputting these files correctly, you can run the degrees.py file, input two actors' names, and the program will return the degree of separation, and each movie that separates them

If using only the small sample given, after inputting Miles Teller and Ryan Gosling, the program will return: 
  
	2 degrees of separation:
  	1: Miles Teller and J.K. Simmons starred in Whiplash
  	2: J.K. Simmons and Ryan Gosling starred in La La Land

