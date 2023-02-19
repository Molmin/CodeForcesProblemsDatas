## Description

<div><p>Your working week consists of $n$ days numbered from $1$ to $n$, after day $n$ goes day $1$ again. And $3$ of them are days off. One of the days off is the last day, day $n$. You have to decide when the other two are.</p><p>Choosing days off, you pursue two goals: </p><ul> <li> No two days should go one after the other. Note that you can't make day $1$ a day off because it follows day $n$. </li><li> Working segments framed by days off should be as dissimilar as possible in duration. More specifically, if the segments are of size $l_1$, $l_2$, and $l_3$ days long, you want to maximize $\min(|l_1 - l_2|, |l_2 - l_3|, |l_3 - l_1|)$. </li></ul><p>Output the maximum value of $\min(|l_1 - l_2|, |l_2 - l_3|, |l_3 - l_1|)$ that can be obtained.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains the integer $n$ ($6 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, output one integer — the maximum possible obtained value.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$) — the number of test cases. The description of test cases follows.</p><p>The only line of each test case contains the integer $n$ ($6 \le n \le 10^9$).</p>

## Output

<p>For each test case, output one integer — the maximum possible obtained value.</p>





```input1|2,4
3
6
10
1033
```




```output1
0
1
342
```



## Note

<p>In the image below you can see the example solutions for the first two test cases. Chosen days off are shown in purple. Working segments are underlined in green.</p><p>In test case $1$, the only options for days off are days $2$, $3$, and $4$ (because $1$ and $5$ are next to day $n$). So the only way to place them without selecting neighboring days is to choose days $2$ and $4$. Thus, $l_1 = l_2 = l_3 = 1$, and the answer $\min(|l_1 - l_2|, |l_2 - l_3|, |l_3 - l_1|) = 0$. </p><center> <img class="tex-graphics" src="file://haheaU7H.png" style="max-width: 100.0%;max-height: 100.0%;" width="832px"> </center><p>For test case $2$, one possible way to choose days off is shown. The working segments have the lengths of $2$, $1$, and $4$ days. So the minimum difference is $1 = \min(1, 3, 2) = \min(|2 - 1|, |1 - 4|, |4 - 2|)$. It can be shown that there is no way to make it larger. </p><center> <img class="tex-graphics" src="file://ou3rbVIY.png" style="max-width: 100.0%;max-height: 100.0%;" width="832px"> </center>
