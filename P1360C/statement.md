## Description

<div><p>We call two numbers $x$ and $y$ <span class="tex-font-style-it">similar</span> if they have the same parity (the same remainder when divided by $2$), or if $|x-y|=1$. For example, in each of the pairs $(2, 6)$, $(4, 3)$, $(11, 7)$, the numbers are similar to each other, and in the pairs $(1, 4)$, $(3, 12)$, they are not.</p><p>You are given an array $a$ of $n$ ($n$ is even) positive integers. Check if there is such a partition of the array into pairs that each element of the array belongs to exactly one pair and the numbers in each pair are similar to each other.</p><p>For example, for the array $a = [11, 14, 16, 12]$, there is a partition into pairs $(11, 12)$ and $(14, 16)$. The numbers in the first pair are similar because they differ by one, and in the second pair because they are both even.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines.</p><p>The first line contains an <span class="tex-font-style-bf">even</span> positive integer $n$ ($2 \le n \le 50$)&nbsp;— length of array $a$.</p><p>The second line contains $n$ positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$).</p></div><div class="output-specification"><p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if the such a partition exists, </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>The letters in the words <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> can be displayed in any case.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of two lines.</p><p>The first line contains an <span class="tex-font-style-bf">even</span> positive integer $n$ ($2 \le n \le 50$)&nbsp;— length of array $a$.</p><p>The second line contains $n$ positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$).</p>

## Output

<p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if the such a partition exists, </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>The letters in the words <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> can be displayed in any case.</p>





```input1
7
4
11 14 16 12
2
1 8
4
1 1 1 1
4
1 2 5 6
2
12 13
6
1 6 3 10 5 8
6
1 12 3 10 5 8
```




```output1
YES
NO
YES
YES
YES
YES
NO
```



## Note

<p>The first test case was explained in the statement.</p><p>In the second test case, the two given numbers are not similar.</p><p>In the third test case, any partition is suitable.</p>
