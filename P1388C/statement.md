## Description

<div><p><span class="tex-font-style-it">Uncle Bogdan is in captain Flint's crew for a long time and sometimes gets nostalgic for his homeland. Today he told you how his country introduced a happiness index.</span></p><p>There are $n$ cities and $n−1$ undirected roads connecting pairs of cities. Citizens of any city can reach any other city traveling by these roads. Cities are numbered from $1$ to $n$ and the city $1$ is a capital. In other words, the country has a tree structure.</p><p>There are $m$ citizens living in the country. A $p_i$ people live in the $i$-th city but all of them are working in the capital. At evening all citizens return to their home cities using the shortest paths. </p><p>Every person has its own mood: somebody leaves his workplace in good mood but somebody are already in bad mood. Moreover any person can ruin his mood on the way to the hometown. <span class="tex-font-style-bf">If person is in bad mood he won't improve it</span>.</p><p>Happiness detectors are installed in each city to monitor the happiness of <span class="tex-font-style-bf">each</span> person who visits the city. The detector in the $i$-th city calculates a happiness index $h_i$ as the number of people in good mood minus the number of people in bad mood. Let's say for the simplicity that <span class="tex-font-style-it">mood of a person doesn't change inside the city</span>.</p><p>Happiness detector is still in development, so there is a probability of a mistake in judging a person's happiness. One late evening, when all citizens successfully returned home, the government asked uncle Bogdan (the best programmer of the country) to check the correctness of the collected happiness indexes.</p><p>Uncle Bogdan successfully solved the problem. Can you do the same?</p><p>More formally, <span class="tex-font-style-it">You need to check: "Is it possible that, after all people return home, for each city $i$ the happiness index will be equal exactly to $h_i$".</span></p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 10^5$; $0 \le m \le 10^9$)&nbsp;— the number of cities and citizens.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_{n}$ ($0 \le p_i \le m$; $p_1 + p_2 + \ldots + p_{n} = m$), where $p_i$ is the number of people living in the $i$-th city.</p><p>The third line contains $n$ integers $h_1, h_2, \ldots, h_{n}$ ($-10^9 \le h_i \le 10^9$), where $h_i$ is the calculated happiness index of the $i$-th city.</p><p>Next $n − 1$ lines contain description of the roads, one per line. Each line contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$; $x_i \neq y_i$), where $x_i$ and $y_i$ are cities connected by the $i$-th road.</p><p>It's guaranteed that the sum of $n$ from all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span>, if the collected data is correct, or <span class="tex-font-style-tt">NO</span>&nbsp;— otherwise. You can print characters in <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> in any case.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n \le 10^5$; $0 \le m \le 10^9$)&nbsp;— the number of cities and citizens.</p><p>The second line of each test case contains $n$ integers $p_1, p_2, \ldots, p_{n}$ ($0 \le p_i \le m$; $p_1 + p_2 + \ldots + p_{n} = m$), where $p_i$ is the number of people living in the $i$-th city.</p><p>The third line contains $n$ integers $h_1, h_2, \ldots, h_{n}$ ($-10^9 \le h_i \le 10^9$), where $h_i$ is the calculated happiness index of the $i$-th city.</p><p>Next $n − 1$ lines contain description of the roads, one per line. Each line contains two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$; $x_i \neq y_i$), where $x_i$ and $y_i$ are cities connected by the $i$-th road.</p><p>It's guaranteed that the sum of $n$ from all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span>, if the collected data is correct, or <span class="tex-font-style-tt">NO</span>&nbsp;— otherwise. You can print characters in <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> in any case.</p>





```input1
2
7 4
1 0 1 1 0 1 0
4 0 0 -1 0 -1 0
1 2
1 3
1 4
3 5
3 6
3 7
5 11
1 2 5 2 1
-11 -2 -6 -2 -1
1 2
1 3
1 4
3 5
```




```input2
2
4 4
1 1 1 1
4 1 -3 -1
1 2
1 3
1 4
3 13
3 3 7
13 1 4
1 2
1 3
```




```output1
YES
YES
```




```output2
NO
NO
```



## Note

<p>Let's look at the first test case of the first sample: </p><center> <img class="tex-graphics" src="file://392w9fAo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>At first, all citizens are in the capital. Let's describe one of possible scenarios: </p><ul> <li> a person from city $1$: he lives in the capital and is in good mood; </li><li> a person from city $4$: he visited cities $1$ and $4$, his mood was ruined between cities $1$ and $4$; </li><li> a person from city $3$: he visited cities $1$ and $3$ in good mood; </li><li> a person from city $6$: he visited cities $1$, $3$ and $6$, his mood was ruined between cities $1$ and $3$; </li></ul> In total, <ul> <li> $h_1 = 4 - 0 = 4$, </li><li> $h_2 = 0$, </li><li> $h_3 = 1 - 1 = 0$, </li><li> $h_4 = 0 - 1 = -1$, </li><li> $h_5 = 0$, </li><li> $h_6 = 0 - 1 = -1$, </li><li> $h_7 = 0$. </li></ul><p>The second case of the first test: </p><center> <img class="tex-graphics" src="file://AA3EgB15.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>All people have already started in bad mood in the capital&nbsp;— this is the only possible scenario.</p><p>The first case of the second test: </p><center> <img class="tex-graphics" src="file://BoYFLJsP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The second case of the second test: </p><center> <img class="tex-graphics" src="file://f2ZjZzGN.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>It can be proven that there is no way to achieve given happiness indexes in both cases of the second test. </p>
