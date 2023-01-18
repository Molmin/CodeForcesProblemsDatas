## Description

<div><p>Phoenix has decided to become a scientist! He is currently investigating the growth of bacteria.</p><p>Initially, on day $1$, there is one bacterium with mass $1$.</p><p>Every day, some number of bacteria will split (possibly zero or all). When a bacterium of mass $m$ splits, it becomes two bacteria of mass $\frac{m}{2}$ each. For example, a bacterium of mass $3$ can split into two bacteria of mass $1.5$.</p><p>Also, every night, the mass of every bacteria will increase by one.</p><p>Phoenix is wondering if it is possible for the total mass of all the bacteria to be exactly $n$. If it is possible, he is interested in the way to obtain that mass using the minimum possible number of nights. Help him become the best scientist!</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 10^9$)&nbsp;— the sum of bacteria masses that Phoenix is interested in. </p></div><div class="output-specification"><p>For each test case, if there is no way for the bacteria to exactly achieve total mass $n$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print two lines.</p><p>The first line should contain an integer $d$ &nbsp;— the minimum number of nights needed.</p><p>The next line should contain $d$ integers, with the $i$-th integer representing the number of bacteria that should split on the $i$-th day.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($2 \le n \le 10^9$)&nbsp;— the sum of bacteria masses that Phoenix is interested in. </p>

## Output

<p>For each test case, if there is no way for the bacteria to exactly achieve total mass $n$, print <span class="tex-font-style-tt">-1</span>. Otherwise, print two lines.</p><p>The first line should contain an integer $d$ &nbsp;— the minimum number of nights needed.</p><p>The next line should contain $d$ integers, with the $i$-th integer representing the number of bacteria that should split on the $i$-th day.</p><p>If there are multiple solutions, print any.</p>





```input1
3
9
11
2
```




```output1
3
1 0 2 
3
1 1 2
1
0
```



## Note

<p>In the first test case, the following process results in bacteria with total mass $9$: </p><ul> <li> Day $1$: The bacterium with mass $1$ splits. There are now two bacteria with mass $0.5$ each. </li><li> Night $1$: All bacteria's mass increases by one. There are now two bacteria with mass $1.5$. </li><li> Day $2$: None split. </li><li> Night $2$: There are now two bacteria with mass $2.5$. </li><li> Day $3$: Both bacteria split. There are now four bacteria with mass $1.25$. </li><li> Night $3$: There are now four bacteria with mass $2.25$. </li></ul> The total mass is $2.25+2.25+2.25+2.25=9$. It can be proved that $3$ is the minimum number of nights needed. There are also other ways to obtain total mass 9 in 3 nights.<p>$ $</p><p>In the second test case, the following process results in bacteria with total mass $11$: </p><ul> <li> Day $1$: The bacterium with mass $1$ splits. There are now two bacteria with mass $0.5$. </li><li> Night $1$: There are now two bacteria with mass $1.5$. </li><li> Day $2$: One bacterium splits. There are now three bacteria with masses $0.75$, $0.75$, and $1.5$. </li><li> Night $2$: There are now three bacteria with masses $1.75$, $1.75$, and $2.5$. </li><li> Day $3$: The bacteria with mass $1.75$ and the bacteria with mass $2.5$ split. There are now five bacteria with masses $0.875$, $0.875$, $1.25$, $1.25$, and $1.75$. </li><li> Night $3$: There are now five bacteria with masses $1.875$, $1.875$, $2.25$, $2.25$, and $2.75$. </li></ul> The total mass is $1.875+1.875+2.25+2.25+2.75=11$. It can be proved that $3$ is the minimum number of nights needed. There are also other ways to obtain total mass 11 in 3 nights.<p>$ $</p><p>In the third test case, the bacterium does not split on day $1$, and then grows to mass $2$ during night $1$.</p>
