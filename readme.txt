
# Word Ladder Puzzle Solver
## Project Overview
The **Word Ladder Puzzle Solver** is a tool that leverages graph theory and Dijkstra’s shortest path algorithm to find the most efficient transformation path between two words. The objective of this puzzle is to transform one word into another by changing only one letter at a time, with the rule that each intermediate word must be a valid entry


## Transformation Rules

 -   **Ladder Step**: In each step, only one character can be changed. The cost of each transformation is determined by the alphabetic distance between the old and new characters.
      -   **Example**: _those_ → _these_ (cost = 10, as 'o' and 'e' differ by 8 letters).
-   **Elevator Step**: This step allows transformation between words that are anagrams of each other. The transformation cost for this step is zero.
    
    -   **Example**: _there_ → _three_ (cost = 0).
 
 ## Features
1.  **Search Functionality**: Enables users to search for words that begin with a specified prefix.
2.  **Neighbor Search**: Allows users to view all neighboring words (words that differ by one letter) for a given word.
3.  **Word Ladder Solver**: Users can input two words, and the program will compute the shortest transformation path between them using both ladder and elevator steps. 

## Requirements


This program is developed in Java and requires a vocabulary file to operate. You can either create your own vocabulary file or use the provided files:

-   **Small file**: `words_250.txt` contains 250 words, suitable for testing the program.
-   **Large file**: `words_5757.txt` contains 5,757 words.

**Note**: Without a vocabulary file, the program will not run, as it requires reading the file from the computer.
