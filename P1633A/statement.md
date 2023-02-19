## Description

<div><p>You are given an integer $n$. You have to change the minimum number of digits in it in such a way that the resulting number <span class="tex-font-style-bf">does not have any leading zeroes</span> and <span class="tex-font-style-bf">is divisible by $7$</span>.</p><p>If there are multiple ways to do it, print any of them. If the given number is already divisible by $7$, leave it unchanged.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 990$) — the number of test cases.</p><p>Then the test cases follow, each test case consists of one line containing one integer $n$ ($10 \le n \le 999$).</p></div><div class="output-specification"><p>For each test case, print one integer without any leading zeroes — the result of your changes (i. e. the integer that is divisible by $7$ and can be obtained by changing the minimum possible number of digits in $n$).</p><p>If there are multiple ways to apply changes, print any resulting number. If the given number is already divisible by $7$, just print it.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 990$) — the number of test cases.</p><p>Then the test cases follow, each test case consists of one line containing one integer $n$ ($10 \le n \le 999$).</p>

## Output

<p>For each test case, print one integer without any leading zeroes — the result of your changes (i. e. the integer that is divisible by $7$ and can be obtained by changing the minimum possible number of digits in $n$).</p><p>If there are multiple ways to apply changes, print any resulting number. If the given number is already divisible by $7$, just print it.</p>





```input1
3
42
23
377
```




```output1
42
28
777
```



## Note

<p>In the first test case of the example, $42$ is already divisible by $7$, so there's no need to change it.</p><p>In the second test case of the example, there are multiple answers — $28$, $21$ or $63$.</p><p>In the third test case of the example, other possible answers are $357$, $371$ and $378$. Note that you <span class="tex-font-style-bf">cannot</span> print $077$ or $77$.</p>
