## Description

<div><p>The sequence $a$ is sent over the network as follows:</p><ol> <li> sequence $a$ is split into segments (each element of the sequence belongs to exactly one segment, each segment is a group of consecutive elements of sequence); </li><li> for each segment, its length is written next to it, either to the left of it or to the right of it; </li><li> the resulting sequence $b$ is sent over the network. </li></ol><p>For example, we needed to send the sequence $a = [1, 2, 3, 1, 2, 3]$. Suppose it was split into segments as follows: $[\color{red}{1}] + [\color{blue}{2, 3, 1}] + [\color{green}{2, 3}]$. Then we could have the following sequences: </p><ul> <li> $b = [1, \color{red}{1}, 3, \color{blue}{2, 3, 1}, \color{green}{2, 3}, 2]$, </li><li> $b = [\color{red}{1}, 1, 3, \color{blue}{2, 3, 1}, 2, \color{green}{2, 3}]$, </li><li> $b = [\color{red}{1}, 1, \color{blue}{2, 3, 1}, 3, 2, \color{green}{2, 3}]$, </li><li> $b = [\color{red}{1}, 1,\color{blue}{2, 3, 1}, 3, \color{green}{2, 3}, 2]$. </li></ul><p>If a different segmentation had been used, the sent sequence might have been different.</p><p>The sequence $b$ is given. Could the sequence $b$ be sent over the network? In other words, is there such a sequence $a$ that converting $a$ to send it over the network could result in a sequence $b$?</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines.</p><p>The first line of the test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the sequence $b$.</p><p>The second line of test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the sequence $b$ itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if sequence $b$ could be sent over the network, that is, if sequence $b$ could be obtained from some sequence $a$ to send $a$ over the network. </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive response).</p></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case consists of two lines.</p><p>The first line of the test case contains an integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the size of the sequence $b$.</p><p>The second line of test case contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the sequence $b$ itself.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case print on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if sequence $b$ could be sent over the network, that is, if sequence $b$ could be obtained from some sequence $a$ to send $a$ over the network. </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as positive response).</p>





```input1|2,3,6,7,10,11,14,15
7
9
1 1 2 3 1 3 2 2 3
5
12 1 2 7 5
6
5 7 8 9 10 3
4
4 8 6 2
2
3 1
10
4 6 2 1 9 4 9 3 4 2
1
1
```




```output1
YES
YES
YES
NO
YES
YES
NO
```



## Note

<p>In the first case, the sequence $b$ could be obtained from the sequence $a = [1, 2, 3, 1, 2, 3]$ with the following partition: $[\color{red}{1}] + [\color{blue}{2, 3, 1}] + [\color{green}{2, 3}]$. The sequence $b$: $[\color{red}{1}, 1, \color{blue}{2, 3, 1}, 3, 2, \color{green}{2, 3}]$.</p><p>In the second case, the sequence $b$ could be obtained from the sequence $a = [12, 7, 5]$ with the following partition: $[\color{red}{12}] + [\color{green}{7, 5}]$. The sequence $b$: $[\color{red}{12}, 1, 2, \color{green}{7, 5}]$.</p><p>In the third case, the sequence $b$ could be obtained from the sequence $a = [7, 8, 9, 10, 3]$ with the following partition: $[\color{red}{7, 8, 9, 10, 3}]$. The sequence $b$: $[5, \color{red}{7, 8, 9, 10, 3}]$.</p><p>In the fourth case, there is no sequence $a$ such that changing $a$ for transmission over the network could produce a sequence $b$.</p>
