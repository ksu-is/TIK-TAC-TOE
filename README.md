# TIK-TAC-TOE
TIK TAC TOE GAME
First project ipython 3
1) Move count = count + 1 after users have made position choice. The reason for this is because if we do count = count + 1 before users have made position choices, count is immediately offset to 1 for userone.
This will affect function replacement_choice() as userone is checked by seeing if count is even or not. 
2) In function gameon_choice2, add a parameter called playername. This is because this line of code:
This line of code assumes that player one will always choose “x” as their symbol. In reality, player one can be “o”. The if statement then becomes:print("Game own! by " + playername + " ({})".format(checksym))
3)Once game is over (either playerone or playertwo wins), ask if players want to replay the game. If the player chooses yes, reset the game, clear the board and play again.
In order to do this, we create game_on_first and game_on_second to see if any player wins or not. If game_on_first or game_on_second is false, which means one of 2 players win, we reset and ask players if they want to replay by calling playertwochoice()
Besides, this will terminate the game immediately if one of the two players wins.

