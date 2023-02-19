## Description

<div><p>Berland crossword is a puzzle that is solved on a square grid with $n$ rows and $n$ columns. Initially all the cells are white.</p><p>To solve the puzzle one has to color some cells on the border of the grid black in such a way that: </p><ul> <li> exactly $U$ cells in the top row are black; </li><li> exactly $R$ cells in the rightmost column are black; </li><li> exactly $D$ cells in the bottom row are black; </li><li> exactly $L$ cells in the leftmost column are black. </li></ul><p>Note that you can color zero cells black and leave every cell white.</p><p>Your task is to check if there exists a solution to the given puzzle.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains $5$ integers $n, U, R, D, L$ ($2 \le n \le 100$; $0 \le U, R, D, L \le n$).</p></div><div class="output-specification"><p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if the solution exists and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The only line of each testcase contains $5$ integers $n, U, R, D, L$ ($2 \le n \le 100$; $0 \le U, R, D, L \le n$).</p>

## Output

<p>For each testcase print "<span class="tex-font-style-tt">YES</span>" if the solution exists and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> are all recognized as positive answer).</p>





```input1
4
5 2 5 3 1
3 0 0 0 0
4 4 1 4 0
2 1 1 1 1
```




```output1
YES
YES
NO
YES
```



## Note

<p>Here are possible solutions to testcases $1$, $2$ and $4$: </p><center> <img class="tex-graphics" src="file://vio1NP5N.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
