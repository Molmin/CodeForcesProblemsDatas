## Description

<div><p>You are given a string $s$ of length $n$, which consists only of the first $k$ letters of the Latin alphabet. All letters in string $s$ are uppercase.</p><p>A <span class="tex-font-style-it">subsequence</span> of string $s$ is a string that can be derived from $s$ by deleting some of its symbols without changing the order of the remaining symbols. For example, "<span class="tex-font-style-tt">ADE</span>" and "<span class="tex-font-style-tt">BD</span>" are subsequences of "<span class="tex-font-style-tt">ABCDE</span>", but "<span class="tex-font-style-tt">DEA</span>" is not.</p><p>A subsequence of $s$ called <span class="tex-font-style-it">good</span> if the number of occurences of each of the first $k$ letters of the alphabet is the same.</p><p>Find the length of the longest good subsequence of $s$. </p></div><div class="input-specification"><p>The first line of the input contains integers $n$ ($1\le n \le 10^5$) and $k$ ($1 \le k \le 26$).</p><p>The second line of the input contains the string $s$ of length $n$. String $s$ only contains uppercase letters from '<span class="tex-font-style-tt">A</span>' to the $k$-th letter of Latin alphabet.</p></div><div class="output-specification"><p>Print the only integer&nbsp;— the length of the longest good subsequence of string $s$.</p></div>

## Input

<p>The first line of the input contains integers $n$ ($1\le n \le 10^5$) and $k$ ($1 \le k \le 26$).</p><p>The second line of the input contains the string $s$ of length $n$. String $s$ only contains uppercase letters from '<span class="tex-font-style-tt">A</span>' to the $k$-th letter of Latin alphabet.</p>

## Output

<p>Print the only integer&nbsp;— the length of the longest good subsequence of string $s$.</p>





```input1
9 3
ACAABCCAB

```




```input2
9 4
ABCABCABC

```




```output1
6
```




```output2
0
```



## Note

<p>In the first example, "<span class="tex-font-style-tt">ACBCAB</span>" ("<span class="tex-font-style-tt"><span class="tex-font-style-bf">AC</span>AA<span class="tex-font-style-bf">BC</span>C<span class="tex-font-style-bf">AB</span></span>") is one of the subsequences that has the same frequency of '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">C</span>'. Subsequence "<span class="tex-font-style-tt">CAB</span>" also has the same frequency of these letters, but doesn't have the maximum possible length.</p><p>In the second example, none of the subsequences can have '<span class="tex-font-style-tt">D</span>', hence the answer is $0$.</p>
