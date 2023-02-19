## Description

<div><p>Alice and Bob are playing a game on a matrix, consisting of $2$ rows and $m$ columns. The cell in the $i$-th row in the $j$-th column contains $a_{i, j}$ coins in it.</p><p>Initially, both Alice and Bob are standing in a cell $(1, 1)$. They are going to perform a sequence of moves to reach a cell $(2, m)$.</p><p>The possible moves are: </p><ul> <li> Move right&nbsp;— from some cell $(x, y)$ to $(x, y + 1)$; </li><li> Move down&nbsp;— from some cell $(x, y)$ to $(x + 1, y)$. </li></ul><p>First, Alice makes <span class="tex-font-style-bf">all her moves</span> until she reaches $(2, m)$. She collects the coins in all cells she visit (including the starting cell).</p><p>When Alice finishes, Bob starts his journey. He also performs the moves to reach $(2, m)$ and collects the coins in all cells that he visited, <span class="tex-font-style-bf">but Alice didn't</span>.</p><p>The score of the game is the total number of coins Bob collects.</p><p>Alice wants to minimize the score. Bob wants to maximize the score. What will the score of the game be if both players play optimally?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of the testcase contains a single integer $m$ ($1 \le m \le 10^5$)&nbsp;— the number of columns of the matrix.</p><p>The $i$-th of the next $2$ lines contain $m$ integers $a_{i,1}, a_{i,2}, \dots, a_{i,m}$ ($1 \le a_{i,j} \le 10^4$)&nbsp;— the number of coins in the cell in the $i$-th row in the $j$-th column of the matrix.</p><p>The sum of $m$ over all testcases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each testcase print a single integer&nbsp;— the score of the game if both players play optimally.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of the testcase contains a single integer $m$ ($1 \le m \le 10^5$)&nbsp;— the number of columns of the matrix.</p><p>The $i$-th of the next $2$ lines contain $m$ integers $a_{i,1}, a_{i,2}, \dots, a_{i,m}$ ($1 \le a_{i,j} \le 10^4$)&nbsp;— the number of coins in the cell in the $i$-th row in the $j$-th column of the matrix.</p><p>The sum of $m$ over all testcases doesn't exceed $10^5$.</p>

## Output

<p>For each testcase print a single integer&nbsp;— the score of the game if both players play optimally.</p>





```input1
3
3
1 3 7
3 5 1
3
1 3 9
3 5 1
1
4
7
```




```output1
7
8
0
```



## Note

<p>The paths for the testcases are shown on the following pictures. Alice's path is depicted in red and Bob's path is depicted in blue.</p><center> <img class="tex-graphics" src="file://Kyd0ilV9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
