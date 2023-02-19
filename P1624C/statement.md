## Description

<div><p>You are given an array $a$ consisting of $n$ positive integers. You can perform operations on it.</p><p>In one operation you can replace any element of the array $a_i$ with $\lfloor \frac{a_i}{2} \rfloor$, that is, by an integer part of dividing $a_i$ by $2$ (rounding down).</p><p>See if you can apply the operation some number of times (possible $0$) to make the array $a$ become a permutation of numbers from $1$ to $n$&nbsp;—that is, so that it contains all numbers from $1$ to $n$, each exactly once.</p><p>For example, if $a = [1, 8, 25, 2]$, $n = 4$, then the answer is yes. You could do the following:</p><ol> <li> Replace $8$ with $\lfloor \frac{8}{2} \rfloor = 4$, then $a = [1, 4, 25, 2]$. </li><li> Replace $25$ with $\lfloor \frac{25}{2} \rfloor = 12$, then $a = [1, 4, 12, 2]$. </li><li> Replace $12$ with $\lfloor \frac{12}{2} \rfloor = 6$, then $a = [1, 4, 6, 2]$. </li><li> Replace $6$ with $\lfloor \frac{6}{2} \rfloor = 3$, then $a = [1, 4, 3, 2]$. </li></ol></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases.</p><p>Each test case contains exactly two lines. The first one contains an integer $n$ ($1 \le n \le 50$), the second one contains integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>For each test case, output on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if you can make the array $a$ become a permutation of numbers from $1$ to $n$, </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;—the number of test cases.</p><p>Each test case contains exactly two lines. The first one contains an integer $n$ ($1 \le n \le 50$), the second one contains integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p>

## Output

<p>For each test case, output on a separate line:</p><ul> <li> <span class="tex-font-style-tt">YES</span> if you can make the array $a$ become a permutation of numbers from $1$ to $n$, </li><li> <span class="tex-font-style-tt">NO</span> otherwise. </li></ul><p>You can output <span class="tex-font-style-tt">YES</span> and <span class="tex-font-style-tt">NO</span> in any case (for example, strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will be recognized as a positive response).</p>





```input1
6
4
1 8 25 2
2
1 1
9
9 8 3 4 2 7 1 5 6
3
8 2 1
4
24 7 16 7
5
22 6 22 4 22
```




```output1
YES
NO
YES
NO
NO
YES
```



## Note

<p>The first test case is explained in the text of the problem statement.</p><p>In the second test case, it is not possible to get a permutation.</p>
