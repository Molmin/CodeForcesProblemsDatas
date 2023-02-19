## Description

<div><p>Define the score of some binary string $T$ as the absolute difference between the number of zeroes and ones in it. (for example, $T=$ <span class="tex-font-style-tt">010001</span> contains $4$ zeroes and $2$ ones, so the score of $T$ is $|4-2| = 2$).</p><p>Define the creepiness of some binary string $S$ as the maximum score among all of its prefixes (for example, the creepiness of $S=$ <span class="tex-font-style-tt">01001</span> is equal to $2$ because the score of the prefix $S[1 \ldots 4]$ is $2$ and the rest of the prefixes have a score of $2$ or less).</p><p>Given two integers $a$ and $b$, construct a binary string consisting of $a$ zeroes and $b$ ones with the minimum possible creepiness.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1\le t\le 1000)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $a$ and $b$ ($ 1 \le a, b \le 100$) &nbsp;— the numbers of zeroes and ones correspondingly.</p></div><div class="output-specification"><p>For each test case, print a binary string consisting of $a$ zeroes and $b$ ones with the minimum possible creepiness. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1\le t\le 1000)$ &nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains two integers $a$ and $b$ ($ 1 \le a, b \le 100$) &nbsp;— the numbers of zeroes and ones correspondingly.</p>

## Output

<p>For each test case, print a binary string consisting of $a$ zeroes and $b$ ones with the minimum possible creepiness. If there are multiple answers, print any of them.</p>





```input1
5
1 1
1 2
5 2
4 5
3 7
```




```output1
10
011
0011000
101010101
0001111111
```



## Note

<p>In the first test case, the score of $S[1 \ldots 1]$ is $1$, and the score of $S[1 \ldots 2]$ is $0$.</p><p>In the second test case, the minimum possible creepiness is $1$ and one of the other answers is <span class="tex-font-style-tt">101</span>.</p><p>In the third test case, the minimum possible creepiness is $3$ and one of the other answers is <span class="tex-font-style-tt">0001100</span>.</p>
