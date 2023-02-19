## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>There is a grid of $n\times m$ cells. Two treasure chests are buried in two different cells of the grid. Your task is to find both of them. You can make two types of operations:  </p><ul> <li> <span class="tex-font-style-tt">DIG $r$ $c$</span>: try to find the treasure in the cell $(r, c)$. The interactor will tell you if you found the treasure or not. </li><li> <span class="tex-font-style-tt">SCAN $r$ $c$</span>: scan from the cell $(r, c)$. The result of this operation is the sum of Manhattan distances from the cell $(r, c)$ to the cells where the treasures are hidden. Manhattan distance from a cell $(r_1, c_1)$ to a cell $(r_2, c_2)$ is calculated as $|r_1 - r_2| + |c_1 - c_2|$. </li></ul><p>You need to find the treasures in at most 7 operations. This includes both <span class="tex-font-style-tt">DIG</span> and <span class="tex-font-style-tt">SCAN</span> operations in total. To solve the test you need to call <span class="tex-font-style-tt">DIG</span> operation at least once in both of the cells where the treasures are hidden.</p></div><div><h2>Interaction</h2><p>Your program has to process multiple test cases in a single run. First, the testing system writes $t$&nbsp;— the number of test cases ($1\le t \le 100$). Then, $t$ test cases should be processed one by one.</p><p>In each test case, your program should start by reading the integers $n$ and $m$ ($2 \le n, m \le 16$).</p><p>Then, your program can make queries of two types:</p><p> </p><ul> <li> <span class="tex-font-style-tt">DIG $r$ $c$</span> ($1\le r\le n$; $1\le c\le m$). The interactor responds with integer $1$, if you found the treasure, and $0$ if not. If you try to find the treasure in the same cell multiple times, the result will be $0$ since the treasure is already found. </li><li> <span class="tex-font-style-tt">SCAN $r$ $c$</span> ($1\le r\le n$; $1\le c\le m$). The interactor responds with an integer that is the sum of Manhattan distances from the cell $(r, c)$ to the cells where the treasures were hidden. The sum is calculated for both cells with treasures, even if you already found one of them. </li></ul><p>After you found both treasures, i.&nbsp;e. you received $1$ for two <span class="tex-font-style-tt">DIG</span> operations, your program should continue to the next test case or exit if that test case was the last one. </p></div>





```input1
1
2 3

1

1

3

0

1
```




```output1
SCAN 1 2

DIG 1 2

SCAN 2 2

DIG 1 1

DIG 1 3
```


