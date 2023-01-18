## Description

<div><p>Berland has $n$ cities, some of which are connected by roads. Each road is bidirectional, connects two distinct cities and for each two cities there's at most one road connecting them.</p><p>The president of Berland decided to split country into $r$ states in such a way that each city will belong to exactly one of these $r$ states.</p><p>After this split each road will connect either cities of the same state or cities of the different states. Let's call roads that connect two cities of the same state "<span class="tex-font-style-it">inner</span>" roads.</p><p>The president doesn't like odd people, odd cities and odd numbers, so he wants this split to be done in such a way that each city would have even number of "<span class="tex-font-style-it">inner</span>" roads connected to it.</p><p>Please help president to find smallest possible $r$ for which such a split exists.</p></div><div class="input-specification"><p>The input contains one or several test cases. The first input line contains a single integer number $t$ — number of test cases. Then, $t$ test cases follow. Solve test cases separately, test cases are completely independent and do not affect each other.</p><p>Then $t$ blocks of input data follow. Each block starts from empty line which separates it from the remaining input data. The second line of each block contains two space-separated integers $n$, $m$ ($1 \le n \le 2000$, $0 \le m \le 10000$) — the number of cities and number of roads in the Berland. Each of the next $m$ lines contains two space-separated integers — $x_i$, $y_i$ ($1 \le x_i, y_i \le n$; $x_i \ne y_i$), which denotes that the $i$-th road connects cities $x_i$ and $y_i$. Each pair of cities are connected by at most one road. </p><p>Sum of values $n$ across all test cases doesn't exceed $2000$. Sum of values $m$ across all test cases doesn't exceed $10000$.</p></div><div class="output-specification"><p>For each test case first print a line containing a single integer $r$ — smallest possible number of states for which required split is possible. In the next line print $n$ space-separated integers in range from $1$ to $r$, inclusive, where the $j$-th number denotes number of state for the $j$-th city. If there are multiple solutions, print any.</p></div>

## Input

<p>The input contains one or several test cases. The first input line contains a single integer number $t$ — number of test cases. Then, $t$ test cases follow. Solve test cases separately, test cases are completely independent and do not affect each other.</p><p>Then $t$ blocks of input data follow. Each block starts from empty line which separates it from the remaining input data. The second line of each block contains two space-separated integers $n$, $m$ ($1 \le n \le 2000$, $0 \le m \le 10000$) — the number of cities and number of roads in the Berland. Each of the next $m$ lines contains two space-separated integers — $x_i$, $y_i$ ($1 \le x_i, y_i \le n$; $x_i \ne y_i$), which denotes that the $i$-th road connects cities $x_i$ and $y_i$. Each pair of cities are connected by at most one road. </p><p>Sum of values $n$ across all test cases doesn't exceed $2000$. Sum of values $m$ across all test cases doesn't exceed $10000$.</p>

## Output

<p>For each test case first print a line containing a single integer $r$ — smallest possible number of states for which required split is possible. In the next line print $n$ space-separated integers in range from $1$ to $r$, inclusive, where the $j$-th number denotes number of state for the $j$-th city. If there are multiple solutions, print any.</p>





```input1
2
&nbsp;
5 3
1 2
2 5
1 5
&nbsp;
6 5
1 2
2 3
3 4
4 2
4 1

```




```output1
1
1 1 1 1 1 
2
2 1 1 1 1 1

```


