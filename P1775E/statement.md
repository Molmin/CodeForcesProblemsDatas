## Description

<div><p>Petya and his friend, the robot Petya++, went to BFDMONCON, where the costume contest is taking place today. </p><center> <img class="tex-graphics" src="file://V4KDcS2s.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>While walking through the festival, they came across a scientific stand named after Professor Oak and Golfball, where they were asked to solve an interesting problem.</p><p>Given a sequence of numbers $a_1, a_2, \dots, a_n$ you can perform several operations on this sequence.</p><p>Each operation should look as follows. You choose some subsequence$^\dagger$. Then you call all the numbers at odd positions in this subsequence <span class="tex-font-style-it">northern</span>, and all the numbers at even positions in this subsequence <span class="tex-font-style-it">southern</span>. In this case, only the position of the number in the subsequence is taken into account, not in the original sequence.</p><p>For example, consider the sequence $1, 4, 2, 8, 5, 7, 3, 6, 9$ and its subsequence (shown in bold) $1, \mathbf{4}, \mathbf{2}, 8, \mathbf{5}, 7, 3, \mathbf{6}, 9$. Then the numbers $4$ and $5$ are <span class="tex-font-style-it">northern</span>, and the numbers $2$ and $6$ are <span class="tex-font-style-it">southern</span>.</p><p>After that, you can do one of the following: </p><ul> <li> add $1$ to all northern numbers and subtract $1$ from all south numbers; or </li><li> add $1$ to all southern numbers and subtract $1$ from all northern numbers. </li></ul><p>Thus, from the sequence $1, \mathbf{4}, \mathbf{2}, 8, \mathbf{5}, 7, 3, \mathbf{6}, 9$, if you choose the subsequence shown in bold, you can get either $1, \mathbf{5}, \mathbf{1}, 8, \mathbf{6}, 7, 3, \mathbf{5}, 9$ or $1, \mathbf{3}, \mathbf{3}, 8, \mathbf{4}, 7, 3, \mathbf{7}, 9$.</p><p>Then the operation ends. Note also that all operations are independent, i.&nbsp;e. the numbers are no longer called <span class="tex-font-style-it">northern</span> or <span class="tex-font-style-it">southern</span> when one operation ends.</p><p>It is necessary to turn all the numbers of the sequence into zeros using the operations described above. Since there is very little time left before the costume contest, the friends want to know, what is the minimum number of operations required for this.</p><p>The friends were unable to solve this problem, so can you help them?</p><p>$^\dagger$ A sequence $c$ is a subsequence of a sequence $d$ if $c$ can be obtained from $d$ by the deletion of several (possibly, zero or all) elements.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2\cdot 10^5$)&nbsp;— the length of the sequence.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the description of the sequence itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer in a single line&nbsp;— the minimum number of operations it takes to turn all the numbers into zeros.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \le n \le 2\cdot 10^5$)&nbsp;— the length of the sequence.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$)&nbsp;— the description of the sequence itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot 10^5$.</p>

## Output

<p>For each test case, print one integer in a single line&nbsp;— the minimum number of operations it takes to turn all the numbers into zeros.</p>





```input1|2,3,6,7,10,11
5
3
1 2 -3
5
1 0 0 -1 -1
6
2 -4 3 -5 4 1
5
1 -1 1 -1 1
7
0 0 0 0 0 0 0
```




```output1
3
2
6
1
0
```



## Note

<p>In the first test case, the sequence of operations is as follows: $\mathbf{1}, 2, \mathbf{-3} \longrightarrow 0, \mathbf{2}, \mathbf{-2} \longrightarrow 0, \mathbf{1}, \mathbf{-1} \longrightarrow 0, 0, 0$.</p><p>In the second test case, the sequence looks like this: $\mathbf{1}, 0, 0, \mathbf{-1}, -1 \longrightarrow 0, 0, 0, 0, \mathbf{-1} \longrightarrow 0, 0, 0, 0, 0$.</p><p>In the fourth test case, simply select the entire sequence as a subsequence, then subtract one from the northern numbers and add one to the southern numbers. Thus, the sequence will be nulled in one operation.</p><p>In the fifth test case, you don't need to do any operations, since the sequence already consists of zeros.</p>
