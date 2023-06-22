# Solitaire
My Javascript version of the Solitaire game

13th Jun: Added basic HTML. Added 4 foundation cards, 7 board cards and the deck together with a new card.
Also added some basic CSS and began researching how to add SVG to cards.
Found that all solitaire playing cards are available as Unicode characters.

16th Jun: Added Card Object class, added all 52 cards as Card's.
Created Array out of all cards.
Added shuffle function, to shuffle all cards in random order.
Created first loop to colour cards either red or black when displayed.

ADD NEXT: change IDs of all board card slots to linear numbers, remove unneeded space, start adding extra rows of cards to board.

19th Jun: Added buttons to show deck card on foundations.
Created all 52 cards on board, pushed non-starting cards to deck array.
Applied colour change to board cards not in front.

Changed font size of non-front cards to keep text away from view.
Created functions to move cards from deck to board, deck to foundation cards and foundation back to the board.
Created max card amount on board (each of the 7 columns being at max 13+7 cards, total 140).

ADD NEXT: Allow only Aces to move to foundation initially, block attempts to move wrong cards to foundation, make sure all functions allow colour change.

20th Jun: Allowed Aces to move to foundation initially, from both the board and the deck. 
All functions now allow colour change.
FIX NEXT: cards that are not ace are not moving from deck to foundation.

All cards now move to foundation properly.
Deck cards now change colour on both types of moves.
When deck cards move to foundation, card is hidden and next card is shown. If no card left, moving button for row disappears.

ADD NEXT: win function with victory changes, reset button and function, when moving deck to board have the correct column chosen to move to and add card to that column, code cleaning required.

21st Jun:
started on checking value function for moving from deck to board.

ADD NEXT: victory function for div, reset function for div, continue moveCheck function, when moving deck to board have the correct column chosen to move to and add card to that column, code cleaning required, move between columns and copy ids and html.

Began reworking entire game around ID Array, where all 140 possible slots on board have ID value in Array, as well as deck and foundation. With foundation to be added.

ADD NEXT: add victory function activation to move to foundation and board to foundation,
modify all functions to use permArrayID and cardArrayA,
code cleaning required,
add move between board buttons and function
modify all buttons to use matching function, with move to and move from column taking precedence, move to requiring function for deck to board & board to board & board to found & found to board

22 June: Code cleaning partially completed.
Tried working on deck to board with mixed results.
Large rewrite of functions required.

ADD NEXT: add victory function activation to move to foundation and board to foundation,
modify all functions to use permArrayID and cardArrayA,
add move between board buttons and function
modify all buttons to use matching function, with move to and move from column taking precedence, move to requiring function for deck to board & board to board & board to found & found to board,
add div to show results of testing, to replace console log.

Moving to requiring function for deck to board.
Created divs to show result of testing.
Began testing deck to board and have moved to columns successfully.
Tested deck emptying with success.

ADD NEXT: add victory function activation to move to foundation and board to foundation,
continue modifying all functions to use permArrayID and cardArrayA,
add move between board functions,
modify all buttons to use matching function, with move to and move from column taking precedence, finish on matching for deck to board, 
start on matching board to board & board to found & found to board.