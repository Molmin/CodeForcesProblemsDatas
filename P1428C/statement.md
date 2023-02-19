## Description

<div><p>Zookeeper is playing a game. In this game, Zookeeper must use bombs to bomb a string that consists of letters '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">B</span>'. He can use bombs to bomb a substring which is either "<span class="tex-font-style-tt">AB</span>" or "<span class="tex-font-style-tt">BB</span>". When he bombs such a substring, the substring gets deleted from the string and the remaining parts of the string get concatenated.</p><p>For example, Zookeeper can use two such operations: <span class="tex-font-style-tt">AAB</span><span class="tex-font-style-underline"><span class="tex-font-style-tt">AB</span></span><span class="tex-font-style-tt">BA</span> $\to$ <span class="tex-font-style-tt">AA</span><span class="tex-font-style-underline"><span class="tex-font-style-tt">BB</span></span><span class="tex-font-style-tt">A</span> $\to$ <span class="tex-font-style-tt">AAA</span>.</p><p>Zookeeper wonders what the shortest string he can make is. Can you help him find the length of the shortest string?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 20000)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>Each of the next $t$ lines contains a single test case each, consisting of a non-empty string $s$: the string that Zookeeper needs to bomb. It is guaranteed that all symbols of $s$ are either '<span class="tex-font-style-tt">A</span>' or '<span class="tex-font-style-tt">B</span>'.</p><p>It is guaranteed that the sum of $|s|$ (length of $s$) among all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer: the length of the shortest string that Zookeeper can make.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ $(1 \leq t \leq 20000)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>Each of the next $t$ lines contains a single test case each, consisting of a non-empty string $s$: the string that Zookeeper needs to bomb. It is guaranteed that all symbols of $s$ are either '<span class="tex-font-style-tt">A</span>' or '<span class="tex-font-style-tt">B</span>'.</p><p>It is guaranteed that the sum of $|s|$ (length of $s$) among all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer: the length of the shortest string that Zookeeper can make.</p>





```input1
3
AAA
BABA
AABBBABBBB
```




```output1
3
2
0
```



## Note

<p>For the first test case, you can't make any moves, so the answer is $3$.</p><p>For the second test case, one optimal sequence of moves is <span class="tex-font-style-tt">B</span><span class="tex-font-style-underline"><span class="tex-font-style-tt">AB</span></span><span class="tex-font-style-tt">A</span> $\to$ <span class="tex-font-style-tt">BA</span>. So, the answer is $2$.</p><p>For the third test case, one optimal sequence of moves is <span class="tex-font-style-tt">AABBBAB<span class="tex-font-style-underline">BB</span>B</span> $\to$ <span class="tex-font-style-tt">AABBB<span class="tex-font-style-underline">AB</span>B</span> $\to$ <span class="tex-font-style-tt">A<span class="tex-font-style-underline">AB</span>BBB</span> $\to$ <span class="tex-font-style-tt">A<span class="tex-font-style-underline">BB</span>B</span> $\to$ <span class="tex-font-style-tt"><span class="tex-font-style-underline">AB</span></span> $\to$ (empty string). So, the answer is $0$.</p>
