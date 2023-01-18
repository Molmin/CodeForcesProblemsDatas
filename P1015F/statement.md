## Description

<div><p>You are given a bracket sequence $s$ (not necessarily a regular one). A bracket sequence is a string containing only characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p><p>A regular bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">+</span>' between the original characters of the sequence. For example, bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"), and "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not.</p><p>Your problem is to calculate the number of regular bracket sequences of length $2n$ containing the given bracket sequence $s$ as a substring (consecutive sequence of characters) modulo $10^9+7$ ($1000000007$).</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 100$) — the half-length of the resulting regular bracket sequences (the resulting sequences must have length equal to $2n$).</p><p>The second line of the input contains one string $s$ ($1 \le |s| \le 200$) — the string $s$ that should be a substring in each of the resulting regular bracket sequences ($|s|$ is the length of $s$).</p></div><div class="output-specification"><p>Print only one integer — the number of regular bracket sequences containing the given bracket sequence $s$ as a substring. Since this number can be huge, print it modulo $10^9+7$ ($1000000007$).</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 100$) — the half-length of the resulting regular bracket sequences (the resulting sequences must have length equal to $2n$).</p><p>The second line of the input contains one string $s$ ($1 \le |s| \le 200$) — the string $s$ that should be a substring in each of the resulting regular bracket sequences ($|s|$ is the length of $s$).</p>

## Output

<p>Print only one integer — the number of regular bracket sequences containing the given bracket sequence $s$ as a substring. Since this number can be huge, print it modulo $10^9+7$ ($1000000007$).</p>





```input1
5
()))()

```




```input2
3
(()

```




```input3
2
(((

```




```output1
5

```




```output2
4

```




```output3
0

```



## Note

<p>All regular bracket sequences satisfying the conditions above for the first example: </p><ul> <li> "<span class="tex-font-style-tt">(((()))())</span>"; </li><li> "<span class="tex-font-style-tt">((()()))()</span>"; </li><li> "<span class="tex-font-style-tt">((()))()()</span>"; </li><li> "<span class="tex-font-style-tt">(()(()))()</span>"; </li><li> "<span class="tex-font-style-tt">()((()))()</span>". </li></ul><p>All regular bracket sequences satisfying the conditions above for the second example: </p><ul> <li> "<span class="tex-font-style-tt">((()))</span>"; </li><li> "<span class="tex-font-style-tt">(()())</span>"; </li><li> "<span class="tex-font-style-tt">(())()</span>"; </li><li> "<span class="tex-font-style-tt">()(())</span>". </li></ul><p>And there is no regular bracket sequences of length $4$ containing "<span class="tex-font-style-tt">(((</span>" as a substring in the third example.</p>
