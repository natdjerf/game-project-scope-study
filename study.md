# Game Project Scope Study

## Required Readings

-   [Game Project](https://github.com/ga-wdi-boston/game-project)
-   [Game API](https://github.com/ga-wdi-boston/game-project-api)
-   [What is a User Story](http://searchsoftwarequality.techtarget.com/definition/user-story)

## Deliverables

After reading the `game-project` prompt and the `game-project-api` documentation
please do the following and be prepared to share and discuss on Monday morning.

Submit detailed answers to these in this file via a pull request.

## A wireframe of what your game project will look like.

Attached separately.

## The data structure you plan to use.

It will be very simple. The sign in, sign out, and change password functionalities will be text fields similar to what we did in class last week. The board displayed on the browser will be HTML and set in place with CSS.

jQuery will be used for tracking user interaction with the browser. As a player selects a location on the screen for his move, events (clicks) will be recorded and communicated using AJAX.

The logic of the game will be in javascript. The board will be a two dimensional array and a function will be written to determine the winner. A player move count will be kept. Ideally, a win count will also be kept.


##  How you will take the markup of the game board and represent it in JS

The logic will first be written using varibles. Once I've completed the AJAX and jQuery to retrieve the appropriate objects, the variables will be based off user interaction with the browers.

The board will be a two dimensional array consisting of 9 pairs of coordinates.
A move counter will be initiated at first play.

Using a function, each move will assign the array with the coordinates, with an 'x' or an 'o'. The move will also trigger an addition to the move count.

When the move counter hits 5, and after every move following, run a callback function to check for a winner. If there is no winner returned, 'next move' will be console logged. If no winner is returned at 9, a tie will be returned. Once the winner/tie is returned, the move count and board will the reset to 0 and the coordinates.

An addition will be added to the player scoreboard.

##  How you plan to approach this project.

Keeping it as simple possible.

First, create a very simple wireframe of how I envision the app to look with all of the requirements (board, sign in/out, change password).

With an idea of what it looks like, walk through how a user would interact with site and map out all possible interactions, as well as the outcome of those moves. Play out each possible outcome and how that information will be recorded. See user-flows.md.

Put together a very basic HTML file to include the sign in/sign out/change password forms and the tic-tac-toe board. Write only the CSS necessary to render the 3x3 board game visible.

Using javascript for the game logic, write a function that will deteremine the winner. The javascript logic will be written out assuming the inputs are variables for testing. Once it's been tested and functioning as expected, it will need to be revised with the inputs using jQuery and AJAX.

After the logic is set, I'll work on user interaction on the site. Simliar to the work we did Friday with jQuery using clicks and hovers to get/set values for both the sign in and board games. I think this will be the most challenging and time consuming part.

Once I can retrieve and populate data from the browswer, I'll work on the AJAX and curl to use the data recieved with jQuery in the game, and update and communicate with the JS.

My main focus is making sure the app is working as expected and efficient. Once I'm comfortable with that I'll work on improving the user experience by updating the UI with CSS.

When it's finalized, I'll put together the documentation with the accurate information necessary.


##  4-8 user stories for your game project.

As a player, I want to easily sign into my account and start a tic-tac-toe with an opponent.

As a player, I want to visualize what the board would look like if I were to play a move before selecting the location.
> I think this can be done with jQuery for a hover or a click and submit.

As a player, I want to see clearly who has won the game.

As a player, I want to keep track of the games played per session and outcomes (wins, ties, opponent wins).
> I'm hoping to store the user's token until he signs out so that after the game so that a scoreboard can be kept.


##  How you plan to keep your code moodular.
As I go through iterations of updating the code, I'm hoping to make it more efficient by using as little hard code as necessary and using callback functions so that no one function consists of too much functionality.


##  What creative spin will you add to your project.
I think this will come as I progress through the project. I think the scoreboard will be the creative spin.

##  How you will use version control to backup / track your project.

Each file will be stored in a different directory the HTML/CSS/jQuery/AJAX etc for organization.
Using the grunt server, I'll test each line of code/ function as I work through them. I anticipate heavy use of console logging and the debugger.

Once tested, I'll commit between each major steps as a way to track progress. I don't think there is a such thing as over committing, and as I anticipate a lot of revisions and interations will be necessary, it will be best that each 'version' is stored.

##  Do you plan to attempt any of the bonuses.
I'm hoping to nail down the main project before considering the bonuses.
