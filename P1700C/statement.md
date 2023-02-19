## Description

<div><p>Little Leon lives in the forest. He has recently noticed that some trees near his favourite path are withering, while the other ones are overhydrated so he decided to learn how to control the level of the soil moisture to save the trees.</p><p>There are $n$ trees growing near the path, the current levels of moisture of each tree are denoted by the array $a_1, a_2, \dots, a_n$. Leon has learned three abilities which will help him to dry and water the soil.</p><ul> <li> Choose a position $i$ and decrease the level of moisture of the trees $1, 2, \dots, i$ by $1$. </li><li> Choose a position $i$ and decrease the level of moisture of the trees $i, i + 1, \dots, n$ by $1$. </li><li> Increase the level of moisture of all trees by $1$. </li></ul><p>Leon wants to know the minimum number of actions he needs to perform to make the moisture of each tree equal to $0$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$) &nbsp;— the number of test cases. The description of $t$ test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 200\,000$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$) — the initial levels of trees moisture. </p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $200\,000$.</p></div><div class="output-specification"><p>For each test case output a single integer — the minimum number of actions. It can be shown that the answer exists.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$) &nbsp;— the number of test cases. The description of $t$ test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 200\,000$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$) — the initial levels of trees moisture. </p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $200\,000$.</p>

## Output

<p>For each test case output a single integer — the minimum number of actions. It can be shown that the answer exists.</p>





```input1
4
3
-2 -2 -2
3
10 4 7
4
4 -4 4 -4
5
1 -2 3 -4 5
```




```output1
2
13
36
33
```



## Note

<p>In the first test case it's enough to apply the operation of adding $1$ to the whole array $2$ times. </p><p>In the second test case you can apply the operation of decreasing $4$ times on the prefix of length $3$ and get an array $6, 0, 3$. </p><p>After that apply the operation of decreasing $6$ times on the prefix of length $1$ and $3$ times on the suffix of length $1$. In total, the number of actions will be $4 + 6 + 3 = 13$. It can be shown that it's impossible to perform less actions to get the required array, so the answer is $13$. </p>
