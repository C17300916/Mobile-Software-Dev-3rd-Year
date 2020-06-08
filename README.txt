Entertainment Top 10 
--------------------
Student Name: Christopher Brady
Student Number: C17300916

App Description:
----------------
The purpose of this app is to allow a user to view the top 10 movies of any genre.
It is perfect for anyone with an interest in movies as it will show them all of the best rated movies.
The ratings are based off of the ratings given on Imdb which is a very reliable source.
A user can click into movies and get information about them. 
There is also an option to click on a link that opens a google search for that movie. 
A user can also search for movies by name, director or lead actors.
An integral part of the app is the ability of users to add any of the movies in the database to their own favourites list,
where they can add or delete movies they would like to watch.

App Instrucions:
----------------
Home Page: 	-The home page of this app gives the user a brief introduction about the app and and its purpose.
	   	-The user can navigate to other pages of the app using the bottom navigation bar.
		-The bottom navigation bar will highlight what part of the app a user is in.
		-There is also an image button where if a user clicks the imdb icon, it will take the to the imdb website.


Top Ten:	-The Top Ten page shows the name, rating and position of the top 10 movies of the selected genre.
		-These are found by accessing the database and doing a select query with a where clause based on genre.
		-On open the selected genre is "All", so the top 10 movies out of all genres is shown.
		-There is a dropdown spinner at the top of the page that allows the user to pick a genre.
		-Once a genre is picked the list will display the top 10 movies of that genre.
		-The list is displayed using a custom adapter and each list item is clickable.
		-Once a list item is clicked a new intent will be called which opens the movie details activity and passes the movie name to that activity.
		-There is also a bottom navigation bar at the bottom of this page, allowing the user to navigate to other pages.


Search:		-The Search page allows a user to search for a movie by movie title, director name or actor name.
		-On this page there are three edit texts for the three possible searches and a button for each of these.
		-If one of the buttons is clicked the search results activity will be called, and the value entered in the relative edit text will be passed.
		-There is also a bottom navigation bar at the bottom of this page, allowing the user to navigate to other pages.

Search Results:	-The Search Results page displays the relative result of a users search entry in a list.
		-The result is found by accessing the database and using a select query and using a where clause with the relative data required.
		-This List is displayed using a custom adapter and includes the name of the movie and its rating.
		-Each movie in the list is clickable and will open the Movie Details activity when clicked.
		-If there are no results to the search entry, the page will display "No Results Found".

Favourites:	-The Favourites page displays all of the favourites that the user has added.
		-The favourite movies are found by using a select statement to find all of the movies in the favourites table.
		-If there are no movies in the favourites table, "You have no favourites" will be displayed.
		-This List is displayed using a custom adapter and includes the name of the movie and its rating.
		-Each movie in the list is clickable and will open the Movie Details activity when clicked.
		-There is also a bottom navigation bar at the bottom of this page, allowing the user to navigate to other pages.

Movie Details:	-The Movie Details page displays more details about the selected movie and allows you to add or delete it from favourites.
		-The details are gotten from the database using a select from the movies table where the movie name is the same as the one that was passed.
		-The details shown include the name, rating , director, lead actors and plot description.
		-In movie details a user can use the gesture double click anywhere on the page to add or delete a movie from favourites.
		-The movie is indicated to whether or not it is in favourites by the star at the bottom of the page.
		-If the star is black and empty, the movie is not in favourites. If it is yellow, the movie is in favourites.
		-There is also a button on this page for a user to find more details about this movie.
		-When clicked, this button will open a browser and do a google search of the movie name to allow the user to get more details.