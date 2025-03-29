Problem
You are given a Google Doc like this one that contains a list of Unicode characters and their positions in a 2D grid. Your task is to write a function that takes in the URL for such a Google Doc as an argument, retrieves and parses the data in the document, and prints the grid of characters. When printed in a fixed-width font, the characters in the grid will form a graphic showing a sequence of uppercase letters, which is the secret message.

The document specifies the Unicode characters in the grid, along with the x- and y-coordinates of each character.

The minimum possible value of these coordinates is 0. There is no maximum possible value, so the grid can be arbitrarily large.

Any positions in the grid that do not have a specified character should be filled with a space character.

You can assume the document will always have the same format as the example document linked above.

        x-coordinate || Character || y-coordinate
         0            ||         █      ||        0
         0            ||         █      ||        1
         0            ||         █      ||        2
         1             ||         ▀       ||        1
         1             ||         ▀       ||        2
         2             ||        ▀        ||        1
         2             ||        ▀        ||        2
         3             ||        ▀        ||        2
         
For example, the simplified example document linked above draws out the letter 'F':

█▀▀▀
█▀▀ 
█  

Specifications
Your code must be written in Python (preferred) or JavaScript.

You may use external libraries.

You may write helper functions, but there should be one function that:

1. Takes in one argument, which is a string containing the URL for the Google Doc with the input data, AND

2. When called, prints the grid of characters specified by the input data, displaying a graphic of correctly oriented uppercase letters.
