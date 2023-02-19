## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is that the easy version does not require you to output the numbers of the rods to be removed. You can make hacks only if all versions of the problem are solved.</span></p><p>Stitch likes experimenting with different machines with his friend Sparky. Today they built another machine.</p><p>The main element of this machine are $n$ rods arranged along one straight line and numbered from $1$ to $n$ inclusive. Each of these rods must carry an electric charge quantitatively equal to either $1$ or $-1$ (otherwise the machine will not work). Another condition for this machine to work is that the sign-variable sum of the charge on all rods must be zero.</p><p>More formally, the rods can be represented as an array of $n$ numbers characterizing the charge: either $1$ or $-1$. Then the condition must hold: $a_1 - a_2 + a_3 - a_4 + \ldots = 0$, or $\sum\limits_{i=1}^n (-1)^{i-1} \cdot a_i = 0$.</p><p>Sparky charged all $n$ rods with an electric current, but unfortunately it happened that the rods were not charged correctly (the sign-variable sum of the charge is not zero). The friends decided to leave only some of the rods in the machine. Sparky has $q$ questions. In the $i$th question Sparky asks: if the machine consisted only of rods with numbers $l_i$ to $r_i$ inclusive, what minimal number of rods could be removed from the machine so that the sign-variable sum of charges on the remaining ones would be zero? Perhaps the friends got something wrong, and the sign-variable sum is already zero. In that case, you don't have to remove the rods at all.</p><p>If the number of rods is zero, we will assume that the sign-variable sum of charges is zero, that is, we can always remove all rods.</p><p>Help your friends and answer all of Sparky's questions!</p></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two positive integers $n$ and $q$ ($1 \le n, q \le 3 \cdot 10^5$)&nbsp;— the number of rods and the number of questions.</p><p>The second line of each test case contains a non-empty string $s$ of length $n$, where the charge of the $i$-th rod is $1$ if $s_i$ is the "<span class="tex-font-style-tt">+</span>" symbol, or $-1$ if $s_i$ is the "<span class="tex-font-style-tt">-</span>" symbol.</p><p>Each next line from the next $q$ lines contains two positive integers $l_i$ ans $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— numbers, describing Sparky's questions.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$, and the sum of $q$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the minimal number of rods that can be removed.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two positive integers $n$ and $q$ ($1 \le n, q \le 3 \cdot 10^5$)&nbsp;— the number of rods and the number of questions.</p><p>The second line of each test case contains a non-empty string $s$ of length $n$, where the charge of the $i$-th rod is $1$ if $s_i$ is the "<span class="tex-font-style-tt">+</span>" symbol, or $-1$ if $s_i$ is the "<span class="tex-font-style-tt">-</span>" symbol.</p><p>Each next line from the next $q$ lines contains two positive integers $l_i$ ans $r_i$ ($1 \le l_i \le r_i \le n$)&nbsp;— numbers, describing Sparky's questions.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$, and the sum of $q$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the minimal number of rods that can be removed.</p>





```input1
3
14 1
+--++---++-++-
1 14
14 3
+--++---+++---
1 14
6 12
3 10
4 10
+-+-
1 1
1 2
1 3
1 4
2 2
2 3
2 4
3 3
3 4
4 4
```




```output1
2
2
1
0
1
2
1
2
1
2
1
1
2
1
```



## Note

<p>In the first test case for the first query you can remove the rods numbered $5$ and $8$, then the following set of rods will remain: <span class="tex-font-style-tt">+--+--++-++-</span>. It is easy to see that here the sign-variable sum is zero.</p><p>In the second test case:</p><ul> <li> For the first query, we can remove the rods numbered $1$ and $11$, then the following set of rods will remain: <span class="tex-font-style-tt">--++---++---</span>. It is easy to see that here the sign-variable sum is zero. </li><li> For the second query we can remove the rod numbered $9$, then the following set of rods will remain: <span class="tex-font-style-tt">---++-</span>. It is easy to see that here the variable sum is zero. </li><li> For the third query we can not remove the rods at all. </li></ul>
