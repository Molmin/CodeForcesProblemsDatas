## Description

<div><p>You are given three arrays $a$, $b$ and $c$. Initially, array $a$ consists of $n$ elements, arrays $b$ and $c$ are empty.</p><p>You are performing the following algorithm that consists of two steps: </p><ul> <li> Step $1$: while $a$ is not empty, you take <span class="tex-font-style-it">the last element</span> from $a$ and move it <span class="tex-font-style-it">in the middle</span> of array $b$. If $b$ currently has odd length, you can choose: place the element from $a$ to the left or to the right of the middle element of $b$. As a result, $a$ becomes empty and $b$ consists of $n$ elements. </li><li> Step $2$: while $b$ is not empty, you take <span class="tex-font-style-it">the middle element</span> from $b$ and move it <span class="tex-font-style-it">to the end</span> of array $c$. If $b$ currently has even length, you can choose which of two middle elements to take. As a result, $b$ becomes empty and $c$ now consists of $n$ elements. </li></ul> Refer to the Note section for examples.<p>Can you make array $c$ sorted in non-decreasing order?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$)&nbsp;— the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains the single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;— the array $a$ itself.</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test, print <span class="tex-font-style-tt">YES</span> (case-insensitive), if you can make array $c$ sorted in non-decreasing order. Otherwise, print <span class="tex-font-style-tt">NO</span> (case-insensitive).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 2 \cdot 10^4$)&nbsp;— the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains the single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of array $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;— the array $a$ itself.</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test, print <span class="tex-font-style-tt">YES</span> (case-insensitive), if you can make array $c$ sorted in non-decreasing order. Otherwise, print <span class="tex-font-style-tt">NO</span> (case-insensitive).</p>





```input1
3
4
3 1 5 3
3
3 2 1
1
7331
```




```output1
YES
NO
YES
```



## Note

<p>In the first test case, we can do the following for $a = [3, 1, 5, 3]$:</p><p>Step $1$: </p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-right">$a$</td><td class="tex-tabular-border-left tex-tabular-text-align-center">$[3, 1, 5, 3]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[3, 1, 5]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[3, 1]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[3]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[]$</td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right">$b$</td><td class="tex-tabular-border-left tex-tabular-text-align-center">$[]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[\underline{3}]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[3, \underline{5}]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[3, \underline{1}, 5]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[3, \underline{3}, 1, 5]$</td></tr></tbody></table><p></p><p>Step $2$: </p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-right">$b$</td><td class="tex-tabular-border-left tex-tabular-text-align-center">$[3, 3, \underline{1}, 5]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[3, \underline{3}, 5]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[\underline{3}, 5]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[\underline{5}]$</td><td class="tex-tabular-text-align-center">$\Rightarrow$</td><td class="tex-tabular-text-align-center">$[]$</td></tr><tr><td class="tex-tabular-text-align-center tex-tabular-border-right">$c$</td><td class="tex-tabular-border-left tex-tabular-text-align-center">$[]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[1]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[1, 3]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[1, 3, 3]$</td><td class="tex-tabular-text-align-center"></td><td class="tex-tabular-text-align-center">$[1, 3, 3, 5]$</td></tr></tbody></table> As a result, array $c = [1, 3, 3, 5]$ and it's sorted.<p></p>
