## Description

<div><p>You are given an array $a$ of $n$ integers.</p><p>You want to make all elements of $a$ equal to zero by doing the following operation <span class="tex-font-style-bf">exactly three</span> times:</p><ul> <li> Select a segment, for each number in this segment we can add a multiple of $len$ to it, where $len$ is the length of this segment (added integers can be different). </li></ul><p>It can be proven that it is always possible to make all elements of $a$ equal to zero.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 100\,000$): the number of elements of the array.</p><p>The second line contains $n$ elements of an array $a$ separated by spaces: $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>The output should contain six lines representing three operations.</p><p>For each operation, print two lines:</p><ul><p> </p><li> The first line contains two integers $l$, $r$ ($1 \le l \le r \le n$): the bounds of the selected segment.<p> </p></li><li> The second line contains $r-l+1$ integers $b_l, b_{l+1}, \dots, b_r$ ($-10^{18} \le b_i \le 10^{18}$): the numbers to add to $a_l, a_{l+1}, \ldots, a_r$, respectively; $b_i$ should be divisible by $r - l + 1$.</li></ul> </div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 100\,000$): the number of elements of the array.</p><p>The second line contains $n$ elements of an array $a$ separated by spaces: $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$).</p>

## Output

<p>The output should contain six lines representing three operations.</p><p>For each operation, print two lines:</p><ul><p> </p><li> The first line contains two integers $l$, $r$ ($1 \le l \le r \le n$): the bounds of the selected segment.<p> </p></li><li> The second line contains $r-l+1$ integers $b_l, b_{l+1}, \dots, b_r$ ($-10^{18} \le b_i \le 10^{18}$): the numbers to add to $a_l, a_{l+1}, \ldots, a_r$, respectively; $b_i$ should be divisible by $r - l + 1$.</li></ul>





```input1
4
1 3 2 4
```




```output1
1 1 
-1
3 4
4 2
2 4
-3 -6 -6
```


