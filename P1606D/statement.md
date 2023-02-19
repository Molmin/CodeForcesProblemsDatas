## Description

<div><p>You are given a matrix, consisting of $n$ rows and $m$ columns. The $j$-th cell of the $i$-th row contains an integer $a_{ij}$.</p><p>First, you have to color each row of the matrix either red or blue in such a way that <span class="tex-font-style-bf">at least one row is colored red</span> and <span class="tex-font-style-bf">at least one row is colored blue</span>.</p><p>Then, you have to choose an integer $k$ ($1 \le k &lt; m$) and cut the colored matrix in such a way that the first $k$ columns become a separate matrix (the <span class="tex-font-style-it">left</span> matrix) and the last $m-k$ columns become a separate matrix (the <span class="tex-font-style-it">right</span> matrix).</p><p>The coloring and the cut are called <span class="tex-font-style-it">perfect</span> if two properties hold: </p><ul> <li> every red cell in the left matrix contains an integer greater than every blue cell in the left matrix; </li><li> every blue cell in the right matrix contains an integer greater than every red cell in the right matrix. </li></ul><p>Find any perfect coloring and cut, or report that there are none.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($2 \le n, m \le 5 \cdot 10^5$; $n \cdot m \le 10^6$)&nbsp;— the number of rows and the number of columns in the matrix, respectively.</p><p>The $i$-th of the next $n$ lines contains $m$ integers $a_{i1}, a_{i2}, \dots, a_{im}$ ($1 \le a_{ij} \le 10^6$).</p><p>The sum of $n \cdot m$ over all testcases doesn't exceed $10^6$.</p></div><div class="output-specification"><p>For each testcase print an answer. If there are no perfect colorings and cuts in the matrix, then print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, first, print "<span class="tex-font-style-tt">YES</span>". Then a string, consisting of $n$ characters: the $i$-th character should be '<span class="tex-font-style-tt">R</span>' if the $i$-th row is colored red and '<span class="tex-font-style-tt">B</span>' if it's colored blue. The string should contain at least one '<span class="tex-font-style-tt">R</span>' and at least one '<span class="tex-font-style-tt">B</span>'. Finally, print an integer $k$ ($1 \le k &lt; m$)&nbsp;— the number of columns from the left that are cut.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of each testcase contains two integers $n$ and $m$ ($2 \le n, m \le 5 \cdot 10^5$; $n \cdot m \le 10^6$)&nbsp;— the number of rows and the number of columns in the matrix, respectively.</p><p>The $i$-th of the next $n$ lines contains $m$ integers $a_{i1}, a_{i2}, \dots, a_{im}$ ($1 \le a_{ij} \le 10^6$).</p><p>The sum of $n \cdot m$ over all testcases doesn't exceed $10^6$.</p>

## Output

<p>For each testcase print an answer. If there are no perfect colorings and cuts in the matrix, then print "<span class="tex-font-style-tt">NO</span>".</p><p>Otherwise, first, print "<span class="tex-font-style-tt">YES</span>". Then a string, consisting of $n$ characters: the $i$-th character should be '<span class="tex-font-style-tt">R</span>' if the $i$-th row is colored red and '<span class="tex-font-style-tt">B</span>' if it's colored blue. The string should contain at least one '<span class="tex-font-style-tt">R</span>' and at least one '<span class="tex-font-style-tt">B</span>'. Finally, print an integer $k$ ($1 \le k &lt; m$)&nbsp;— the number of columns from the left that are cut.</p>





```input1
3
5 5
1 5 8 8 7
5 2 1 4 3
1 6 9 7 5
9 3 3 3 2
1 7 9 9 8
3 3
8 9 8
1 5 3
7 5 7
2 6
3 3 3 2 2 2
1 1 1 4 4 4
```




```output1
YES
BRBRB 1
NO
YES
RB 3
```



## Note

<p>The coloring and the cut for the first testcase:</p><center> <img class="tex-graphics" src="file://jEzijJPi.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
