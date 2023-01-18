## Description

<div><p>For her birthday Alice received an interesting gift from her friends – The Light Square. The Light Square game is played on an $N \times N$ lightbulbs square board with a magical lightbulb bar of size $N \times 1$ that has magical properties. At the start of the game some lights on the square board and magical bar are turned on. The goal of the game is to transform the starting light square board pattern into some other pattern using the magical bar without rotating the square board. The magical bar works as follows: </p><p>It can be placed on any row or column </p><p>The orientation of the magical lightbulb must be left to right or top to bottom for it to keep its magical properties </p><p>The entire bar needs to be fully placed on a board </p><p>The lights of the magical bar never change </p><p>If the light on the magical bar is the same as the light of the square it is placed on it will switch the light on the square board off, otherwise it will switch the light on </p><p>The magical bar can be used an infinite number of times </p><p>Alice has a hard time transforming her square board into the pattern Bob gave her. Can you help her transform the board or let her know it is impossible? If there are multiple solutions print any. </p></div><div class="input-specification"><p>The first line contains one positive integer number $N\ (1 \leq N \leq 2000)$ representing the size of the square board. </p><p>The next $N$ lines are strings of length $N$ consisting of 1's and 0's representing the initial state of the square board starting from the top row. If the character in a string is 1 it means the light is turned on, otherwise it is off. </p><p>The next $N$ lines are strings of length $N$ consisting of 1's and 0's representing the desired state of the square board starting from the top row that was given to Alice by Bob. </p><p>The last line is one string of length $N$ consisting of 1's and 0's representing the pattern of the magical bar in a left to right order. </p></div><div class="output-specification"><p>Transform the instructions for Alice in order to transform the square board into the pattern Bob gave her. The first line of the output contains an integer number $M\ (0 \leq M \leq 10^5$) representing the number of times Alice will need to apply the magical bar. </p><p>The next $M$ lines are of the form "col $X$" or "row $X$", where $X$ is $0$-based index of the matrix, meaning the magical bar should be applied to either row $X$ or column $X$. If there is no solution, print only -1. In case of multiple solutions print any correct one. </p></div>

## Input

<p>The first line contains one positive integer number $N\ (1 \leq N \leq 2000)$ representing the size of the square board. </p><p>The next $N$ lines are strings of length $N$ consisting of 1's and 0's representing the initial state of the square board starting from the top row. If the character in a string is 1 it means the light is turned on, otherwise it is off. </p><p>The next $N$ lines are strings of length $N$ consisting of 1's and 0's representing the desired state of the square board starting from the top row that was given to Alice by Bob. </p><p>The last line is one string of length $N$ consisting of 1's and 0's representing the pattern of the magical bar in a left to right order. </p>

## Output

<p>Transform the instructions for Alice in order to transform the square board into the pattern Bob gave her. The first line of the output contains an integer number $M\ (0 \leq M \leq 10^5$) representing the number of times Alice will need to apply the magical bar. </p><p>The next $M$ lines are of the form "col $X$" or "row $X$", where $X$ is $0$-based index of the matrix, meaning the magical bar should be applied to either row $X$ or column $X$. If there is no solution, print only -1. In case of multiple solutions print any correct one. </p>





```input1
2
11
11
00
01
11
```




```input2
2
10
00
00
00
10
```




```input3
3
110
011
100
100
011
100
100
```




```output1
-1
```




```output2
1
row 0
```




```output3
3
row 0
col 0
col 1
```



## Note

<p>Example 1: It is impossible to transform square board from one format to another</p><p>Example 2: Magic bar can be applied on first row or column.</p>
