## Description

<div><p>Shubham has a binary string $s$. A binary string is a string containing only characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>".</p><p>He can perform the following operation on the string any amount of times: </p><ul> <li> Select an index of the string, and flip the character at that index. This means, if the character was "<span class="tex-font-style-tt">0</span>", it becomes "<span class="tex-font-style-tt">1</span>", and vice versa. </li></ul><p>A string is called good if it does not contain "<span class="tex-font-style-tt">010</span>" or "<span class="tex-font-style-tt">101</span>" as a subsequence &nbsp;— for instance, "<span class="tex-font-style-tt">1001</span>" contains "<span class="tex-font-style-tt">101</span>" as a subsequence, hence it is not a good string, while "<span class="tex-font-style-tt">1000</span>" doesn't contain neither "<span class="tex-font-style-tt">010</span>" nor "<span class="tex-font-style-tt">101</span>" as subsequences, so it is a good string.</p><p>What is the minimum number of operations he will have to perform, so that the string becomes good? It can be shown that with these operations we can make any string good.</p><p>A string $a$ is a subsequence of a string $b$ if $a$ can be obtained from $b$ by deletion of several (possibly, zero or all) characters.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1\le t \le 100)$&nbsp;— the number of test cases.</p><p>Each of the next $t$ lines contains a binary string $s$ $(1 \le |s| \le 1000)$.</p></div><div class="output-specification"><p>For every string, output the minimum number of operations required to make it good.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1\le t \le 100)$&nbsp;— the number of test cases.</p><p>Each of the next $t$ lines contains a binary string $s$ $(1 \le |s| \le 1000)$.</p>

## Output

<p>For every string, output the minimum number of operations required to make it good.</p>





```input1
7
001
100
101
010
0
1
001100
```




```output1
0
0
1
1
0
0
2
```



## Note

<p>In test cases $1$, $2$, $5$, $6$ no operations are required since they are already good strings.</p><p>For the $3$rd test case: "<span class="tex-font-style-tt">001</span>" can be achieved by flipping the first character &nbsp;— and is one of the possible ways to get a good string.</p><p>For the $4$th test case: "<span class="tex-font-style-tt">000</span>" can be achieved by flipping the second character &nbsp;— and is one of the possible ways to get a good string.</p><p>For the $7$th test case: "<span class="tex-font-style-tt">000000</span>" can be achieved by flipping the third and fourth characters &nbsp;— and is one of the possible ways to get a good string.</p>
