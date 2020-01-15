# Memory-Game
A card game of flip-and-match. It consists of multiple options: timed/untimed, with/without rating for the player. The game runs on a PIC16F84A chip.

#Instructions for use
After building the project with MPLAB, open the simulation file and double click on the PIC chip. Locate the HEX file of your project in
the "Program file" space.

The game consists of 6 matching pairs. So, total of 12 cards are available. The cards will be labeled alphabetically from A to F. So,
we will have two cards labeled as A, 2 as B, 2 as C, 2 as D, 2 as E, and 2 as F.  
 
In mode 1: the game will end only if a player makes all matching pairs. So, the player will keep playing until he/she makes
all the available matches (6 matches in our case). Then, depending on the player’s performance (number of non-matching were done
during the game), the player will get a feedback as Super, Average, or Weak. In addition to that, a bar-meter will be shown on the screen
(which is related to number of non-matching) to show the player performance after each turn. The meter will grow from Super (lower number
of non-matching) to Weak (higher number of non-matching) and it will be updated after each turn. More description will be provided later.  
 
In Mode 2: the game will be time dependent. The player should make matching pairs before the end of the game time. Then, the final score
will be provided as a combination of the remaining time and the number of matches done. Also, in this mode, the game ends whenever the
player makes all available matches or the time of game ends.  
 
In mode 3: the game will have different scoring techniques. An initial score will be set. Then every match, a point will be added to
this score. After every non-matching pair, the system will check if the card were revealed before (opened more than one time and failed
to do a match), then a point will be deducted from the score for every re-opened revealed card. Here, the game will end if the player makes
all the available matches or the player reaches the max number of opened revealed cards.

#Authors of this project: Yehya El Hassan, Serine Al Daouk, and myself.
