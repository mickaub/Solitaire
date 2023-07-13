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

23 June: Continued working on deck to board and deck to foundation.
Deck to board is a little buggy but can work, need to work on function to make fully functional.
Need to create match function to use to simplify code.
Added victory is foundations are at max.

Started work on match function. Able to match cards including King, if column empty king able to move.
Most deck functions now working well.

ADD NEXT: Continue work on match function.
Continue modifying functions to use CardArrayA.
Try to take away dependency on PermArray.
Add move between board functions.
Modify all buttons to use matching function, with move to and move from column taking precedence. 
Start on matching board to board & board to found & found to board.

26 Jun: Massive rewrite and simplification of code.
Deck to found has issues and deck to board has issues.

ADD NEXT: Continue work on match function.
Continue modifying functions to use CardArrayA.
Try to take away dependency on PermArray.
Add move between board functions.
Modify all buttons to use matching function, with move to and move from column taking precedence. 
Start on matching board to board & board to found & found to board.

27 June: Began reorganising code, with main focus on permArray, foundationArr and frontPos/frontID arrays. 
Will use arrays within arrays to help match cards, with card matches in matches array to check before moving if match can occur.

ADD NEXT: Continue work on matchtest function.
Start reworking deck functions, beginning with swapdeck.
Add move between board functions. 
Start on matching board to board & board to found & found to board.
Fix CSS that is cutting board in half.

28 June: Began working on match function.
MatchFunction works and shows id that is required to go on top of all board columns and foundation as well.

ADD NEXT: Convert working match loop into function.
Continue working on match function.
Start reworking deck functions, beginning with swapdeck.
Add move between board functions. 
Start on matching board to board & board to found & found to board.
Fix CSS that is cutting board in half.

Fixed CSS isue that was cutting board in half.
MatchArray is now a function.
MatchArray has no objects and is all numbers.
Started working on swapdeck.
All matching functions will use the MatchArray function in some way, including board to board movements.

TO DO: Continue working on swapdeck and other deck functions.
Add move between board functions. 

Reworked deck to foundation function, which is working and updating correctly.
Swapdeck includes move to foundation options.

TO DO: Work on deck to board function.
Amend swap deck to include deck to board options, with matchcombined being used.
Need to add functions to foundation and column buttons.

29 Jun: Deck to Board is functioning, without updating the div colours.
Deck to board works for multiple cards in seperate matches.
Victory condition also works correctly.
Changed formatting to be more readable.

TO DO: Continue with Board to Foundation function.
Add div colour change/check for swapDeck and other Deck functions.
Need to add functions to foundation and column buttons.

Board to Foundation function works, with only the right card moving to the foundation.
Temporarily combined MoveFromBoard and Move To Foundation, in order to move from board to foundation.
Move From Column buttons now have function.

TO DO: Seperate MoveFromBoard and BoardToFound, via storing arguments into a variable, which will then need to be wiped after use.
Begin work on Foundation down to Board.
Add div colour change/check for swapDeck and other Deck functions.
Need to add functions to foundation and move to column buttons.

30 June:
Foundation to Board works, although it only uses the first match.
Changed design so that deck is in the middle of the foundation and the board.

TO DO: 
Work on Board to Board function.
Seperate MoveFromBoard and BoardToFound, via storing arguments into a variable, which will then need to be wiped after use.
Seperate MoveToBoard and FoundToBoard, via storing arguments into a variable, which will then need to be wiped after use.
Need to add selector for multiple foundations, with extra divs that popup/greyin or out.
Add div colour change/check for swapDeck and other Deck functions.

1 July:
Added seperate selections for multiple foundation options.
Got board to board function(through movefromboard) to work correctly.
Fixed king from deck to empty column.
Fixed king from column to empty column.
Added frontbackPos array and have planned how to use.

TO DO:
Add frontbackPos to functions including board to future board to board function. LINE220 PLANNING
Add div colour change/check for swapDeck and other Deck functions, as well as all other buttons and functions.
Add function to board to found buttons.
Add seperate selections of foundToboard and BoardtoFound options into the functions.
Seperate MoveFromBoard and BoardToFound, via storing arguments into a variable, which will then need to be wiped after use.
Seperate moving Board to Board from MoveFromBoard and put some into MoveToBoard.
Seperate MoveToBoard and FoundToBoard, via storing arguments into a variable, which will then need to be wiped after use.
Fix formatting issue with cards above div 52.

3 Jul
Began working on frontbackPos to record the furthest back card that is visible.
frontBackPos works in various functions.
Attempted to start recording the cards in the middle of the front and the last front card, but the calculations were causing issues.

Made checkback function to check all front facing cards that are not the front. Working and outputting ID of the other front facing cards.
Fixed formatting issues with cards above div 52.
Board to Foundation div changes colour to match foundation that can accept new card.
Frontmatch checks for board to found and function clears it.

TODO:
Add to frontmatch function the ability to check found to board, and board to board chance.
Add div colour change/check for swapDeck and other Deck functions, as well as other functions and found to board, move to board, move from column and move to column buttons.
Add function to board to found buttons.
Add seperate selections of foundToboard and BoardtoFound options into the functions.
Seperate MoveFromBoard and BoardToFound, via storing arguments into a variable, which will then need to be wiped after use.
Seperate moving Board to Board from MoveFromBoard and put some into MoveToBoard.
Seperate MoveToBoard and FoundToBoard, via storing arguments into a variable, which will then need to be wiped after use.

4 Jul
Deck to board buttons change div colour when ready and change back.
Seperated movefromboard and boardtofound functions.
Board to Found divs change colour and back again when needed.
Added functions to board to found buttons.
Added seperate selections for boardToFound function.

Adjusted size of moving to and from column buttons.
Worked on foundation to board function.
Foundation to board and move to column change colour when ready.
FoundToBoard function works correctly.
Added to frontMatch the ability to check found to board.

TODO:

Continue working on MoveFromBoard and MoveToBoard functions, especially in relation to multiple layer moves.
Add to frontmatch function the ability to check board to board chance.
Add div colour change/check for move from column and move to column buttons, for interboard transfer.
Rework movetoBoard by allowing it to change the foundation and move the proper foundation card to the correct column.

5 Jul
Fixed Found to Board function, which is working correctly.
Reworked MoveToBoard to differentiate between moving from foundation and moving from board, with the foundation part working correctly.

Added to frontMatch the ability to check board to board chance with one layer of card.
Added div colour change/check for interboard transfer.
MoveFromBoard and MoveToBoard work correctly for moving cards between columns, with only a slight bug.

TODO:

Continue working on MoveFromBoard and MoveToBoard functions in relation to multiple layer moves.
Add to frontmatch function the ability to check board to board chance with multiple layers.
Integrate CheckBack into frontMatch.

6 Jul
Added to frontMatch function the ability to check board to board chances with multiple layers, by adding checkback function.
Working on moving from back to one specific column.

TODO:
Continue working on MoveFromBoard and MoveToBoard functions in relation to multiple layer moves.

7 Jul
TEMPORARY STOP
To improve efficiency, I will be taking a break for a little while and will move back to solitaire in the future.
Current completion: 80%.
When I restart, I will need to focus on:
Moving multiple layers of cards from behind.
Changing Checkback function for multiple layers.
Changing appeareance of move from board and move to board divs for multiple layer moves.
Changing movefromBoard function to accomodate multiple choices per column.
Changing movetoBoard function to accomodate moving multiple cards, and choosing from the multiple recieving columns.

12 Jul
RESTART
Began adding test cards to use when testing multiple moves.

TODO:
Moving multiple layers of cards from behind.
Changing Checkback function for multiple layers.
Changing appearance of move from board and move to board divs for multiple layer moves.
Changing movefromBoard function to accomodate multiple choices per column.
Changing movetoBoard function to accomodate moving multiple cards, and choosing from the multiple recieving columns.

13 Jul
Cleaning code to make moving cards easier.
Focus on FrontMatch, decktoboard, foundtoBoard, 
movefromboard, movetoboard functions.
Inluded new code to move multiple card matches.

Logged covered cards and removed cards from covered array when no longer covered.
MatchingCards lists all matches including ones behind the front.

TODO:
Need to remove duplicates from fromTo array.
L504: replace i with alternative
Remove other behindfront calculations and arrays.
Decide between changing movefromcolarr to accomodate multiple options or using fromTo to display multiple options instead.
Need to set moving amount and moving values in one of the functions.
Need to set multiple values in moveFromColArr result, in FrontBack function.
Reset board to columns and movefromcol array after moves.
Changing appearance of move from board and move to board divs for multiple layer moves.
Reset all moving to/from board divs after move.
Changing movefromBoard function to accomodate multiple choices per column.
Changing movetoBoard function to accomodate moving multiple cards, and choosing from the multiple recieving columns.