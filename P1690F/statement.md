## Description

<div><p>Polycarp found the string $s$ and the permutation $p$. Their lengths turned out to be the same and equal to $n$.</p><p>A permutation of $n$ elements&nbsp;— is an array of length $n$, in which every integer from $1$ to $n$ occurs exactly once. For example, $[1, 2, 3]$ and $[4, 3, 5, 1, 2]$ are permutations, but $[1, 2, 4]$, $[4, 3, 2, 1, 2]$ and $[0, 1, 2]$ are not.</p><p>In one operation he can multiply $s$ by $p$, so he replaces $s$ with string $new$, in which for any $i$ from $1$ to $n$ it is true that $new_i = s_{p_i}$. For example, with $s=wmbe$ and $p = [3, 1, 4, 2]$, after operation the string will turn to $s=s_3 s_1 s_4 s_2=bwem$.</p><p>Polycarp wondered after how many operations the string would become equal to its initial value for the first time. Since it may take too long, he asks for your help in this matter.</p><p>It can be proved that the required number of operations always exists. It can be very large, so use a 64-bit integer type. </p></div><div class="input-specification"><p>The first line of input contains one integer $t$ ($1 \le t \le 5000$) — the number of test cases in input.</p><p>The first line of each case contains single integer $n$ ($1 \le n \le 200$) — the length of string and permutation.</p><p>The second line of each case contains a string $s$ of length $n$, containing lowercase Latin letters.</p><p>The third line of each case contains $n$ integers&nbsp;— permutation $p$ ($1 \le p_i \le n$), all $p_i$ are different.</p></div><div class="output-specification"><p>Output $t$ lines, each of which contains the answer to the corresponding test case of input. As an answer output single integer&nbsp;— the minimum number of operations, after which the string $s$ will become the same as it was before operations.</p></div>

## Input

<p>The first line of input contains one integer $t$ ($1 \le t \le 5000$) — the number of test cases in input.</p><p>The first line of each case contains single integer $n$ ($1 \le n \le 200$) — the length of string and permutation.</p><p>The second line of each case contains a string $s$ of length $n$, containing lowercase Latin letters.</p><p>The third line of each case contains $n$ integers&nbsp;— permutation $p$ ($1 \le p_i \le n$), all $p_i$ are different.</p>

## Output

<p>Output $t$ lines, each of which contains the answer to the corresponding test case of input. As an answer output single integer&nbsp;— the minimum number of operations, after which the string $s$ will become the same as it was before operations.</p>





```input1
3
5
ababa
3 4 5 2 1
5
ababa
2 1 4 5 3
10
codeforces
8 6 1 7 5 2 9 3 10 4
```




```output1
1
6
12
```



## Note

<p>In the first sample operation doesn't change the string, so it will become the same as it was after $1$ operations.</p><p>In the second sample the string will change as follows:</p><ul><li> $s$ = <span class="tex-font-style-tt">babaa</span></li><li> $s$ = <span class="tex-font-style-tt">abaab</span></li><li> $s$ = <span class="tex-font-style-tt">baaba</span></li><li> $s$ = <span class="tex-font-style-tt">abbaa</span></li><li> $s$ = <span class="tex-font-style-tt">baaab</span></li><li> $s$ = <span class="tex-font-style-tt">ababa</span></li></ul>
