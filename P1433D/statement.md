## Description

<div><p>There are $n$ districts in the town, the $i$-th district belongs to the $a_i$-th bandit gang. Initially, no districts are connected to each other.</p><p>You are the mayor of the city and want to build $n-1$ two-way roads to connect all districts (two districts can be connected directly or through other connected districts).</p><p>If two districts belonging to the same gang are connected <span class="tex-font-style-bf">directly</span> with a road, this gang will revolt.</p><p>You don't want this so your task is to build $n-1$ two-way roads in such a way that all districts are reachable from each other (possibly, using intermediate districts) and <span class="tex-font-style-bf">each pair</span> of directly connected districts belong to <span class="tex-font-style-bf">different gangs</span>, or determine that it is impossible to build $n-1$ roads to satisfy all the conditions.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 500$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 5000$) — the number of districts. The second line of the test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the gang the $i$-th district belongs to.</p><p>It is guaranteed that the sum of $n$ does not exceed $5000$ ($\sum n \le 5000$).</p></div><div class="output-specification"><p>For each test case, print:</p><ul> <li> <span class="tex-font-style-tt">NO</span> on the only line if it is impossible to connect all districts satisfying the conditions from the problem statement. </li><li> <span class="tex-font-style-tt">YES</span> on the first line and $n-1$ roads on the next $n-1$ lines. Each road should be presented as a pair of integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n; x_i \ne y_i$), where $x_i$ and $y_i$ are two districts the $i$-th road connects. </li></ul><p>For each road $i$, the condition $a[x_i] \ne a[y_i]$ should be satisfied. Also, all districts should be reachable from each other (possibly, using intermediate districts).</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 500$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 5000$) — the number of districts. The second line of the test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the gang the $i$-th district belongs to.</p><p>It is guaranteed that the sum of $n$ does not exceed $5000$ ($\sum n \le 5000$).</p>

## Output

<p>For each test case, print:</p><ul> <li> <span class="tex-font-style-tt">NO</span> on the only line if it is impossible to connect all districts satisfying the conditions from the problem statement. </li><li> <span class="tex-font-style-tt">YES</span> on the first line and $n-1$ roads on the next $n-1$ lines. Each road should be presented as a pair of integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n; x_i \ne y_i$), where $x_i$ and $y_i$ are two districts the $i$-th road connects. </li></ul><p>For each road $i$, the condition $a[x_i] \ne a[y_i]$ should be satisfied. Also, all districts should be reachable from each other (possibly, using intermediate districts).</p>





```input1
4
5
1 2 2 1 3
3
1 1 1
4
1 1000 101 1000
4
1 2 3 4
```




```output1
YES
1 3
3 5
5 4
1 2
NO
YES
1 2
2 3
3 4
YES
1 2
1 3
1 4
```


