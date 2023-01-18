## Description

<div><p>Oh, no!</p><p>The coronavirus has caught you, and now you're sitting in a dark cellar, with tied legs (but not hands). You have a delicious cookie, a laptop in front of you, and your ideal development environment is open. The coronavirus convinces you to solve the following problem.</p><p>You are given two arrays $A$ and $B$ of size $n$. You can do operations of two types with array $A$: </p><ul> <li> Reverse array $A$. That is the array $[A_1,\ A_2,\ \ldots,\ A_n]$ transformes into $[A_n,\ A_{n-1},\ \ldots,\ A_1]$. </li><li> Replace $A$ with an array of its prefix sums. That is, the array $[A_1,\ A_2,\ \ldots,\ A_n]$ goes to $[A_1,\ (A_1+A_2),\ \ldots,\ (A_1+A_2+\ldots+A_n)]$. </li></ul><p>You need to understand if you can get an array $B$ from the array $A$. If it is possible, you will have to restore the order of these operations by minimizing the number of operations of the second type. Fortunately, the coronavirus is good today, so he has allowed you not to restore actions if the minimum number of second type operations is more than $2\cdot 10^5$. But coronavirus resents you, so if you restore the answer, the total number of operations should not exceed $5\cdot 10^5$.</p><p>Solve this problem and get the cookie, or the coronavirus will extend the quarantine for five years and make the whole economy collapse! </p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1\le n \le 2\cdot 10^5$).</p><p>The second line contains $n$ integers $A_1, A_2, \ldots, A_n$ ($1 \le A_i \le 10 ^ {12}$).</p><p>The third line contains $n$ integers $B_1, B_2, \ldots, B_n$ ($1 \le B_i \le 10 ^ {12}$).</p></div><div class="output-specification"><p>If you cannot get $B$ from the $A$ array, print "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without quotes) on a single line.</p><p>If the minimum number of operations of the second type exceeds $2\cdot 10^5$, print "<span class="tex-font-style-tt">BIG</span>" (without quotes). In the second line print the number of operations of the second type, that needs to be applied to get array $B$ from $A$.</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">SMALL</span>" (without quotes). In the second line print the total number of operations of the first and second types $m \le 5\cdot 10^5$ (it is guaranteed that in this case there is such a sequence of actions). In the third line print a line of length $m$, consisting of characters '<span class="tex-font-style-tt">R</span>"and '<span class="tex-font-style-tt">P</span>' (without quotes).</p><p>The $i$-th character should be '<span class="tex-font-style-tt">R</span>', if the $i$-th action is of the first type, and should be '<span class="tex-font-style-tt">P</span>', otherwise.</p><p>If there are several such sequences, you can print any of them.</p><p>You can print each character in the uppercase or in the lowercase.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1\le n \le 2\cdot 10^5$).</p><p>The second line contains $n$ integers $A_1, A_2, \ldots, A_n$ ($1 \le A_i \le 10 ^ {12}$).</p><p>The third line contains $n$ integers $B_1, B_2, \ldots, B_n$ ($1 \le B_i \le 10 ^ {12}$).</p>

## Output

<p>If you cannot get $B$ from the $A$ array, print "<span class="tex-font-style-tt">IMPOSSIBLE</span>" (without quotes) on a single line.</p><p>If the minimum number of operations of the second type exceeds $2\cdot 10^5$, print "<span class="tex-font-style-tt">BIG</span>" (without quotes). In the second line print the number of operations of the second type, that needs to be applied to get array $B$ from $A$.</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">SMALL</span>" (without quotes). In the second line print the total number of operations of the first and second types $m \le 5\cdot 10^5$ (it is guaranteed that in this case there is such a sequence of actions). In the third line print a line of length $m$, consisting of characters '<span class="tex-font-style-tt">R</span>"and '<span class="tex-font-style-tt">P</span>' (without quotes).</p><p>The $i$-th character should be '<span class="tex-font-style-tt">R</span>', if the $i$-th action is of the first type, and should be '<span class="tex-font-style-tt">P</span>', otherwise.</p><p>If there are several such sequences, you can print any of them.</p><p>You can print each character in the uppercase or in the lowercase.</p>





```input1
2
5 7
5 7
```




```input2
2
1 1
300000 1
```




```input3
2
10 1
13 14
```




```input4
3
1 2 1
2 1 2
```




```output1
SMALL
0
```




```output2
BIG
299999
```




```output3
SMALL
6
RPPPRP
```




```output4
IMPOSSIBLE
```



## Note

<p>In the first example, the arrays $A$ and $B$ already equal, so the number of required operations $=0$.</p><p>In the second example, we need to replace $A$ with the prefix sums $299999$ times and then reverse the array. Since $299999&gt;2\cdot 10^5$, there is no need to restore the answer.</p><p>In the fourth example, you cannot get $B$ from the $A$.</p>
