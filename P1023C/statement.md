## Description

<div><p>A bracket sequence is a string containing only characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". A regular bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example, bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"), and "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not.</p><p><span class="tex-font-style-it">Subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements.</span></p><p>You are given a regular bracket sequence $s$ and an integer number $k$. Your task is to find a regular bracket sequence of length exactly $k$ such that it is also a subsequence of $s$.</p><p>It is guaranteed that such sequence always exists.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le k \le n \le 2 \cdot 10^5$, both $n$ and $k$ are even) — the length of $s$ and the length of the sequence you are asked to find.</p><p>The second line is a string $s$ — regular bracket sequence of length $n$.</p></div><div class="output-specification"><p>Print a single string — a regular bracket sequence of length exactly $k$ such that it is also a subsequence of $s$.</p><p>It is guaranteed that such sequence always exists.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le k \le n \le 2 \cdot 10^5$, both $n$ and $k$ are even) — the length of $s$ and the length of the sequence you are asked to find.</p><p>The second line is a string $s$ — regular bracket sequence of length $n$.</p>

## Output

<p>Print a single string — a regular bracket sequence of length exactly $k$ such that it is also a subsequence of $s$.</p><p>It is guaranteed that such sequence always exists.</p>





```input1
6 4
()(())

```




```input2
8 8
(()(()))

```




```output1
()()

```




```output2
(()(()))

```


