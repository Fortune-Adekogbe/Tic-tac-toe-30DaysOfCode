# Tic-tac-toe-30DaysOfCode


Are you tired of seeing "no inbuilt module should be used"? Say no more...

Today you'll be writing a couple of functions that will collectively render a simple and efficient tic-tac-toe playing environment. To help you with this is the beautiful PyGame library. Most people usually start python with the aim of building Machine Learning Models or doing backend web development but forget that it can also be a powerful tool for game development.
Install pygame with the command:
pip install pygame

To start:
Import the pygame and all its local variables.
initialize pygame
initialize pyGame display variable with pygame.display to your desired size
Also set the caption for the game as "Tic-Tac-Toe".

Before you go on to write your functions setup your global
variables two of which are the player that starts and the 
game grid as a 3 x 3 matrix with null values.

Here are your instructions for the support functions:

# Write a function named initialize_board

    Aim: initialize the background and return it.
    This takes in a properly initialized pyGame display variable as its only parameter.
    With this and pygame's Surface method, set up the background of the board. Also set the color of the background using the RGB format.
    Draw the vertical and horizontal grid lines on the background that partitions the section of the background that is your game board into the expected nine boxes. 
    
Initialize your board by calling the function above.

# Write a function named draw_status
    
    Aim: This function renders the current status (like the players turn and winner) at the bottom of the game board.
    It takes in the already initialized background as its parameter.
    First determine the message to be returned based on the current playing status
    Set font for the message and render the messsage into a variable with pygames methods
    Erase any previous message and copy the rendered message onto the board.
    *Note that the space that is allocated for this should be included during display variable initialisation.*
    
    
# Write a function named show_board
    
    Aim: This function draws/redraws the game board on the display now containing your message.
    It takes in the initialized pyGame display (same one that the first function took) and the background (same as the second functions parameter).
    First it calls the second function thereby adding the message section to the board; then it displays the board.

    

# Write the function board_position

    Aim: Take in a set of coordinates from the mouse as separate parameters and determines which box (row, column) the user clicked.
    It takes in the X and Y coordinates of the mouse clicked point and returns a tuple row and column clicked.
    
# Write a function named depict_move

    Aim: This function draws an X or O on the board in the specified row and column.
    It takes in the board, the row and column to be drawn in as separate parameters and the piece to be drawn.
    The function identifies the piece to be drawn and draws it in the right board space with the pygame.draw functions.
 
    
# Write a function named click_board

    Aim: This is the function that gets the mouse position and activates the depict_move function
    it takes in the play board as parameter, determines where the user clicked and if the space is not already occupied.
    Then it calls the depict_move function to draw the appropriate piece then changes the turn.
    
# Write a function named game_over

    Aim: This function determines if anyone has won the game.
    It takes in the board as a parameter.
    it then checks the different winning conditions and draws a line on the board across the winning path to signify the end of the game.
    
    
# After writing all the support functions:


Using a def main() function to make sure your game only works when it is run inside your script:

Write the main event loop.

    In this using the Pygame.event.get() function, take instructions from your keyboard 
    on whether to play or quit. Show at the top of your scripts what keys you selected for 
    what purpose. 

    Call required functions to:

        -- Determine what area was clicked.
        -- Check for a winner
        -- Update the display so new events are registered

Note that you have to keep the main event loop constantly running for the game to be usable. This should guide you on what loop to use.

*Check out the pygame docs @ https://www.pygame.org/docs/*
