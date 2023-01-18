## Description

<div><p>You are given a special jigsaw puzzle consisting of $n\cdot m$ identical pieces. Every piece has three tabs and one blank, as pictured below.</p><center> <img class="tex-graphics" src="file://vHCTL5kY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The jigsaw puzzle is considered solved if the following conditions hold:</p><ol> <li> The pieces are arranged into a grid with $n$ rows and $m$ columns. </li><li> For any two pieces that share an edge in the grid, a tab of one piece fits perfectly into a blank of the other piece. </li></ol><p>Through rotation and translation of the pieces, determine if it is possible to solve the jigsaw puzzle.</p></div><div class="input-specification"><p>The test consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 1000$)&nbsp;— the number of test cases. Next $t$ lines contain descriptions of test cases.</p><p>Each test case contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$).</p></div><div class="output-specification"><p>For each test case output a single line containing "<span class="tex-font-style-tt">YES</span>" if it is possible to solve the jigsaw puzzle, or "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The test consists of multiple test cases. The first line contains a single integer $t$ ($1\le t\le 1000$)&nbsp;— the number of test cases. Next $t$ lines contain descriptions of test cases.</p><p>Each test case contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$).</p>

## Output

<p>For each test case output a single line containing "<span class="tex-font-style-tt">YES</span>" if it is possible to solve the jigsaw puzzle, or "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case (upper or lower).</p>





```input1
3
1 3
100000 100000
2 2
```




```output1
YES
NO
YES
```



## Note

<p>For the first test case, this is an example solution: </p><center> <img class="tex-graphics" src="file://3ZrlpK9V.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the second test case, we can show that no solution exists.</p><p>For the third test case, this is an example solution:</p><center> <img class="tex-graphics" src="file://x58KXtK6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
