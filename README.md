# Board Games

  1. TicTacToe  
  2. Connect Four  
  3. NTicTacToe  


#How To Run
0. Show help: `java -jar BoardGames.jar`
1. `java -jar BoardGames.jar tic`
2. `java -jar BoardGames.jar ntic`
3. `java -jar BoardGames.jar connect`


# Notes
1. Board is bassed to Game as composition from their respective runner classes (Run*.java) Since there is an inherent assumption about how these games work. So, the client should not have access to changes the rules by creating a custom board.

2. Game has an AbstarctGame because the 3 games have different rules.
3. Board has a concrete class BaseBoard because the properties of a board is not changing much
4. The "AI" is nothing but `Collections.shuffle(moves);`, PlayerA and PlayerB try their luck :)