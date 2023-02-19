## Description

<div><p>You are given an array $a$ of $n$ positive integers. Determine if, by rearranging the elements, you can make the array strictly increasing. In other words, determine if it is possible to rearrange the elements such that $a_1 &lt; a_2 &lt; \dots &lt; a_n$ holds.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if the array satisfies the condition, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 100$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_i$ ($1 \leq a_i \leq 10^9$)&nbsp;— the elements of the array.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if the array satisfies the condition, and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p><p>You can output the answer in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>" and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7
3
4
1 1 1 1
5
8 7 1 3 4
1
5
```




```output1
NO
YES
YES
```



## Note

<p>In the first test case any rearrangement will keep the array $[1,1,1,1]$, which is not strictly increasing.</p><p>In the second test case, you can make the array $[1,3,4,7,8]$.</p>
