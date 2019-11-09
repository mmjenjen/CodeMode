# CodeMode
A fun code review game by Maargaret Jennings and Margaret Flemmings for Wellesley's CS304 Databases with Web Interfaces class. 

## More details
Home page: http://cs.wellesley.edu:7535/ (or substitute your localhost)
Sign in
To create a new user, click on the button “Join Now”.  This will toggle to show an option to add a username and password. Do this and submit - you are now on the main site.
Click on any of the tabs to navigate between pages

Select a Quiz to take: http://cs.wellesley.edu:7535/select/
The drop down menu has been replaced with a carousel, flip through the different quizzes or let the carousel move them for you
Once you have decided on a quiz, click on that slide, you will be sent to the quiz page

Make questions and add them to a Deck: http://cs.wellesley.edu:7535/insertQuestion/
You may add your own, or for example, add

	Question Text: Which of the following is an inline element?
	Answer: <span>
	Answer (type): Multiple Choice
	Wrong Option 1: <div> 
	Wrong Option 2: <li>  
	Wrong Option 3: <header> 
	Explanation: span is the only inline element
	Point value: 1
	Add to deck: HTML
  
If you are adding a “fill in the blank” question, switch using the drop down menu next to Answer Type.
The wrong answers will disappear from the table of inputs to fill out
When finished, click submit where you will be redirected -- only if you fill out everything! -- to a page where you will be able make edits to questions that already exist in the table.
Update Quiz Question: http://cs.wellesley.edu:7535/updateQuestion/10
Update any part of a quiz question to update it in the database

Make or edit the name of an existing Deck (like a deck of cards/questions): http://cs.wellesley.edu:7535/insertDeck/	
Create a new deck/quiz and upload an image to go with the deck on the carousel
One deck is inserted, will redirect so you can update the name of the current deck
Update Deck Name: http://cs.wellesley.edu:7535/updateDeck/2
Update a deck’s name

PHP Deck Quiz: http://cs.wellesley.edu:7535/quiz/3
Shows all the questions that are in the selected deck. 
Use radio buttons to select answers for multiple choices questions, type in text for fill in the blank, and use the submit button to grade your answers. 
The page will check quizzes (given that all questions have been answered) and will grade them, show the user the explanation and if they got it right or wrong, show the points they earned, and the total score. 
All questions are required by the form. 
Updates the points of the current user

Database Tables:
Database: codemode_db
Tables:
Users: stores data for all of the users such as usernames, encrypted passwords, and points
Questions: stores all of the question information, such as the text, answer, explanation, and point value
Decks: stores the names and pictures for all decks
