## Description

<div><p>After getting bored by playing with crayons, you decided to switch to Legos! Today, you're working with a long strip, with height $1$ and length $n$, some positions of which are occupied by $1$ by $1$ Lego pieces.</p><p>In one second, you can either remove two <span class="tex-font-style-it">adjacent</span> Lego pieces from the strip (if both are present), or add two Lego pieces to <span class="tex-font-style-it">adjacent</span> positions (if both are absent). You can only add or remove Lego's at two adjacent positions at the same time, as otherwise your chubby fingers run into precision issues.</p><p>You want to know exactly how much time you'll spend playing with Legos. You value efficiency, so given some starting state and some ending state, you'll always spend the least number of seconds to transform the starting state into the ending state. If it's impossible to transform the starting state into the ending state, you just skip it (so you spend $0$ seconds).</p><p>The issue is that, for some positions, you don't remember whether there were Legos there or not (in either the starting state, the ending state, or both). Over all pairs of (starting state, ending state) that are consistent with your memory, find the total amount of time it will take to transform the starting state to the ending state. Print this value modulo $1\,000\,000\,007$ ($10^9 + 7$). </p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 2000$)&nbsp;— the size of the Lego strip.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>&nbsp;— your memory of the starting state: </p><ul> <li> <span class="tex-font-style-tt">1</span> represents a position that definitely has a Lego piece, </li><li> <span class="tex-font-style-tt">0</span> represents a position that definitely does not have a Lego piece, </li><li> and <span class="tex-font-style-tt">?</span> represents a position that you don't remember. </li></ul><p>The third line of each test case contains a string $t$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>&nbsp;— your memory of the ending state. It follows a similar format to the starting state.</p><p>It's guaranteed that the sum of $n$ over all test cases doesn't exceed $2000$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the answer to the problem modulo $1\,000\,000\,007$ ($10^9 + 7$). </p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 1000$)&nbsp;— the number of test cases. Then $t$ cases follow.</p><p>The first line of each test case contains one integer $n$ ($2 \leq n \leq 2000$)&nbsp;— the size of the Lego strip.</p><p>The second line of each test case contains a string $s$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>&nbsp;— your memory of the starting state: </p><ul> <li> <span class="tex-font-style-tt">1</span> represents a position that definitely has a Lego piece, </li><li> <span class="tex-font-style-tt">0</span> represents a position that definitely does not have a Lego piece, </li><li> and <span class="tex-font-style-tt">?</span> represents a position that you don't remember. </li></ul><p>The third line of each test case contains a string $t$ of length $n$, consisting of the characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, and <span class="tex-font-style-tt">?</span>&nbsp;— your memory of the ending state. It follows a similar format to the starting state.</p><p>It's guaranteed that the sum of $n$ over all test cases doesn't exceed $2000$.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the answer to the problem modulo $1\,000\,000\,007$ ($10^9 + 7$). </p>





```input1
6
2
00
11
3
???
???
3
??1
0?0
4
??0?
??11
5
?????
0??1?
10
?01??01?1?
??100?1???
```




```output1
1
16
1
14
101
1674
```



## Note

<p>For the first test case, $00$ is the only possible starting state, and $11$ is the only possible ending state. It takes exactly one operation to change $00$ to $11$.</p><p>For the second test case, some of the possible starting and ending state pairs are: </p><ul> <li> $(000, 011)$&nbsp;— takes $1$ operation. </li><li> $(001, 100)$&nbsp;— takes $2$ operations. </li><li> $(010, 000)$&nbsp;— takes $0$ operations, as it's impossible to achieve the ending state. </li></ul>
