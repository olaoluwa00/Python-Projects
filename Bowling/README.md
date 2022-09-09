# Bowling Scoring

This question was modified from a tutorial sheet question for the second year of Oxford University's undergraduate engineering course. The task was to "write a programme that correctly scores a single-player game of American 10 pin bowling, following the "traditional" method (https://en.wikipedia.org/wiki/Ten-pin_bowling#Traditional_scoring) as follows":

* Each game of bowling is ten turns, or frames.
* In each frame, the player gets up to two rolls to knock down all ten pins.
* If all the pins are knocked down on the first roll this is called a strike. This ends the frame, and the score for the frame is 10 plus the total of the pins knocked down on next two rolls.
* If the pins are all knocked down in two rolls this is called a spare and the score for the frame is 10 plus the number of pins knocked down on the next roll.
* If the player fails to knock down all the pins in the frame, their score for that frame is the total number of pins knocked down in the two rolls.
* If the player gets a spare or strike in the final (tenth) frame, the player gets to roll one or two more bonus balls, respectively. These bonus rolls are taken as part of the same frame. If a bonus roll knocks down all the pins, the process does not repeat: the bonus rolls are only used to calculate the score of the final frame.
* The game score is the total of all frame scores.

The input to the program was supposed to be a string of characters representing rolls, where "x" indicates a strike, "/" indicates a spare, "-" indicates a miss, else a number represents the number of pins knocked down in that roll. I changed the program so that the score was entered from a graphical user interface, created with Tkinter, and the string which was originally the input was now the output.

I Tested my code on the following inputs:
* XXXXXXXXXXXX : 12 rolls, 12 strikes, therefore 10 frames * 30 points = 300
* 9-9-9-9-9-9-9-9-9-9- : 20 rolls, 10 pairs of 9 and miss, therefore 10 frames * 9 points = 90
* 5/5/5/5/5/5/5/5/5/5/5 : 21 rolls, 10 pairs of 5 and spare, with a final 5 = 10 frames * 15 points
  = 150
