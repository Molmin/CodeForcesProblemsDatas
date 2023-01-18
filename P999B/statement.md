## Description

<div><p>A string $s$ of length $n$ can be encrypted by the following algorithm:</p><ul> <li> iterate over all divisors of $n$ in decreasing order (i.e. from $n$ to $1$), </li><li> for each divisor $d$, reverse the substring $s[1 \dots d]$ (i.e. the substring which starts at position $1$ and ends at position $d$). </li></ul><p>For example, the above algorithm applied to the string $s$="<span class="tex-font-style-tt">codeforces</span>" leads to the following changes: "<span class="tex-font-style-tt">codeforces</span>" $\to$ "<span class="tex-font-style-tt">secrofedoc</span>" $\to$ "<span class="tex-font-style-tt">orcesfedoc</span>" $\to$ "<span class="tex-font-style-tt">rocesfedoc</span>" $\to$ "<span class="tex-font-style-tt">rocesfedoc</span>" (obviously, the last reverse operation doesn't change the string because $d=1$).</p><p>You are given the encrypted string $t$. Your task is to decrypt this string, i.e., to find a string $s$ such that the above algorithm results in string $t$. It can be proven that this string $s$ always exists and is unique.</p></div><div class="input-specification"><p>The first line of input consists of a single integer $n$ ($1 \le n \le 100$) — the length of the string $t$. The second line of input consists of the string $t$. The length of $t$ is $n$, and it consists only of lowercase Latin letters.</p></div><div class="output-specification"><p>Print a string $s$ such that the above algorithm results in $t$.</p></div>

## Input

<p>The first line of input consists of a single integer $n$ ($1 \le n \le 100$) — the length of the string $t$. The second line of input consists of the string $t$. The length of $t$ is $n$, and it consists only of lowercase Latin letters.</p>

## Output

<p>Print a string $s$ such that the above algorithm results in $t$.</p>





```input1
10
rocesfedoc

```




```input2
16
plmaetwoxesisiht

```




```input3
1
z

```




```output1
codeforces

```




```output2
thisisexampletwo

```




```output3
z

```



## Note

<p>The first example is described in the problem statement.</p>
