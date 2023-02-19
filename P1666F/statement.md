## Description

<div><p>Little Fiona has a collection of $n$ blocks of various sizes $a_1, a_2, \ldots, a_n$, where $n$ is even. Some of the blocks can be equal in size. She would like to put all these blocks one onto another to form a <span class="tex-font-style-it">fancy</span> stack.</p><p>Let $b_1, b_2, \ldots, b_n$ be the sizes of blocks in the stack from top to bottom. Since Fiona is using all her blocks, $b_1, b_2, \ldots, b_n$ must be a permutation of $a_1, a_2, \ldots, a_n$. Fiona thinks the stack is <span class="tex-font-style-it">fancy</span> if both of the following conditions are satisfied: </p><ul> <li> The second block is strictly bigger than the first one, and then each block is alternately strictly smaller or strictly bigger than the previous one. Formally, $b_1 &lt; b_2 &gt; b_3 &lt; b_4 &gt; \ldots &gt; b_{n-1} &lt; b_n$. </li><li> The sizes of the blocks on even positions are strictly increasing. Formally, $b_2 &lt; b_4 &lt; b_6 &lt; \ldots &lt; b_n$ (remember that $n$ is even). </li></ul><center> <img class="tex-graphics" src="file://4EpNfZL7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Two stacks are considered different if their corresponding sequences $b_1, b_2, \ldots, b_n$ differ in at least one position.</p><p>Fiona wants to know how many different fancy stacks she can build with all of her blocks. Since large numbers scare Fiona, find this number modulo $998\,244\,353$.</p></div><div class="input-specification"><p>Each input contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2500$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;— the number of blocks at Fiona's disposal ($2 \le n \le 5000$; $n$ is even). The second line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— the sizes of the blocks in non-decreasing order ($1 \le a_1 \le a_2 \le \dotsb \le a_n \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p></div><div class="output-specification"><p>For each test case, print the number of ways to build a fancy stack, modulo $998\,244\,353$.</p></div>

## Input

<p>Each input contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 2500$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$&nbsp;— the number of blocks at Fiona's disposal ($2 \le n \le 5000$; $n$ is even). The second line contains $n$ integers $a_1, a_2, \ldots, a_n$&nbsp;— the sizes of the blocks in non-decreasing order ($1 \le a_1 \le a_2 \le \dotsb \le a_n \le n$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5000$.</p>

## Output

<p>For each test case, print the number of ways to build a fancy stack, modulo $998\,244\,353$.</p>





```input1
2
4
1 2 3 4
8
1 1 2 3 4 4 6 7
```




```output1
2
4
```


