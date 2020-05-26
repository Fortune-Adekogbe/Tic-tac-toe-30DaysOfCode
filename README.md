# Tic-tac-toe-30DaysOfCode


Are you tired of seeing "no inbuilt module should be used"? Say no more...

Today you'll be writing a couple of functions that will collectively render a simple and efficient tic-tac-toe playing environment. To help you with this is the beautiful PyGame library. Most people usually start python with the aim of building Machine Learning Models or doing backend web development but forget that it can also be a powerful tool for game development.
Install pygame with the command:
pip install pygame

To start:

initialize pygame
initialize pyGame display and store in a variable with the pygame.display class
Also set the caption for as "Tic-Tac-Toe" with pygame if you want to.

Here are your instructions for the support functions:

-- Write a function named initialize_board.
    Aim: initialize the background and return it as a variable.
    This takes in a properly initialized pyGame display as its only parameter.
    With this and pygame's Surface method, set up the background of the board.(You can also set the color of the     background)
    Draw the vertical and horizontal grid lines on the background that partitions the section of the background that is your game board into the expected nine boxes. 
    
-- Write a function named draw_status.

    Aim: This function draws the current status (like the players turn and winner) at the bottom of the game board.
    It takes in the already created background as its parameter.
    First determine the message to be returned based on the current playing status
    Set font for the message and render the messsage into a variable with PyGames methods
    Erase any previous message and copy the rendered message onto the board.
    
    Yes, you saw it right, this function returns nothing. Lets move on...
    
-- Write a function named show_board
    
    Aim: This function draws the game board on the display now containing your message.
    It takes in the initialized pyGame display (same one that the first function took) and the board (same as the second functions parameter).
    First it calls the second function thereby adding the message section to the board; then it displays the board.
    

# Write the function board_position

    Aim: Take in a set of coordinates from the mouse as separate parameters and determines which box (row, column) the user clicked.
    It takes in the X and Y coordinates of the mouse clicked point and returns a tuple row and column clicked.
    
# Write a function named depict_move

    Aim: This function draws an X or O on the board in the specified row x column.
    It takes in the board, the row and column to be drawn in as separate parameters and the piece to be drawn.
    The function identifies the piece to be drawn and draws it in the right board space with the pygame.draw functions.
    
    This also returns nothing.
    
# Write a function named click_board

    Aim: This is the function that gets the mouse position and activates the depict_move function
    it takes in the play board as parameter, determines where the user clicked and if the space is not already occupied.
    Then it calls the depict_move function to draw the appropriate piece then changes the turn.
    
# Write a function named game_over

    Aim: This function determines if anyone has won the game.
    It takes in the board as a parameter.
    it then checks the different winning conditions and draws a line on the board across the winning combo to signify the end of a round.
    
    
# After writing all the support functions:

Create the game board with the initialize_board function

Using a def main() function to make sure your game only works inside your script:

Write the main event loop. In this:

    Call required functions to:

        -- Determine what the user clicked and what area was clicked.
        -- Check for a winner
        -- Update the display so new events are registered

Chech out the pygame.event.get() function to determine when a user clicks with the MOUSEBUTTONDOWN or if they want to QUIT.

Check out the pygame docs @ www.pygame.org/docs
