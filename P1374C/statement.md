## Description

<div><p>You are given a bracket sequence $s$ of length $n$, where $n$ is even (divisible by two). The string $s$ consists of $\frac{n}{2}$ opening brackets '<span class="tex-font-style-tt">(</span>' and $\frac{n}{2}$ closing brackets '<span class="tex-font-style-tt">)</span>'.</p><p>In one move, you can choose <span class="tex-font-style-bf">exactly one bracket</span> and move it to the beginning of the string or to the end of the string (i.e. you choose some index $i$, remove the $i$-th character of $s$ and insert it before or after all remaining characters of $s$).</p><p>Your task is to find the minimum number of moves required to obtain <span class="tex-font-style-bf">regular bracket sequence</span> from $s$. It can be proved that the answer always exists under the given constraints.</p><p>Recall what the regular bracket sequence is:</p><ul> <li> "<span class="tex-font-style-tt">()</span>" is regular bracket sequence; </li><li> if $s$ is regular bracket sequence then "<span class="tex-font-style-tt">(</span>" + $s$ + "<span class="tex-font-style-tt">)</span>" is regular bracket sequence; </li><li> if $s$ and $t$ are regular bracket sequences then $s$ + $t$ is regular bracket sequence. </li></ul><p>For example, "<span class="tex-font-style-tt">()()</span>", "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">(())</span>" and "<span class="tex-font-style-tt">()</span>" are regular bracket sequences, but "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">()(</span>" and "<span class="tex-font-style-tt">)))</span>" are not.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 2000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 50$) — the length of $s$. It is guaranteed that $n$ is even. The second line of the test case containg the string $s$ consisting of $\frac{n}{2}$ opening and $\frac{n}{2}$ closing brackets.</p></div><div class="output-specification"><p>For each test case, print the answer — the minimum number of moves required to obtain <span class="tex-font-style-bf">regular bracket sequence</span> from $s$. It can be proved that the answer always exists under the given constraints.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 2000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 50$) — the length of $s$. It is guaranteed that $n$ is even. The second line of the test case containg the string $s$ consisting of $\frac{n}{2}$ opening and $\frac{n}{2}$ closing brackets.</p>

## Output

<p>For each test case, print the answer — the minimum number of moves required to obtain <span class="tex-font-style-bf">regular bracket sequence</span> from $s$. It can be proved that the answer always exists under the given constraints.</p>





```input1
4
2
)(
4
()()
8
())()()(
10
)))((((())
```




```output1
1
0
1
3
```



## Note

<p>In the first test case of the example, it is sufficient to move the first bracket to the end of the string.</p><p>In the third test case of the example, it is sufficient to move the last bracket to the beginning of the string.</p><p>In the fourth test case of the example, we can choose last three openning brackets, move them to the beginning of the string and obtain "<span class="tex-font-style-tt">((()))(())</span>".</p>
