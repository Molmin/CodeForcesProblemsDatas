## Description

<div><p>You are given a bracket sequence $s$ consisting of $n$ opening '<span class="tex-font-style-tt">(</span>' and closing '<span class="tex-font-style-tt">)</span>' brackets.</p><p>A <span class="tex-font-style-it">regular</span> bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">+</span>' between the original characters of the sequence. For example, bracket sequences "<span class="tex-font-style-tt">()()</span>", "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>", "<span class="tex-font-style-tt">((1+1)+1)</span>"), and "<span class="tex-font-style-tt">)(</span>" and "<span class="tex-font-style-tt">(</span>" are not.</p><p>You can change the type of some bracket $s_i$. It means that if $s_i = $ '<span class="tex-font-style-tt">)</span>' then you can change it to '<span class="tex-font-style-tt">(</span>' and vice versa.</p><p>Your task is to calculate the number of positions $i$ such that if you change the type of the $i$-th bracket, then the resulting bracket sequence becomes <span class="tex-font-style-it">regular</span>.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 10^6$) — the length of the bracket sequence.</p><p>The second line of the input contains the string $s$ consisting of $n$ opening '<span class="tex-font-style-tt">(</span>' and closing '<span class="tex-font-style-tt">)</span>' brackets.</p></div><div class="output-specification"><p>Print one integer — the number of positions $i$ such that if you change the type of the $i$-th bracket, then the resulting bracket sequence becomes <span class="tex-font-style-it">regular</span>.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 10^6$) — the length of the bracket sequence.</p><p>The second line of the input contains the string $s$ consisting of $n$ opening '<span class="tex-font-style-tt">(</span>' and closing '<span class="tex-font-style-tt">)</span>' brackets.</p>

## Output

<p>Print one integer — the number of positions $i$ such that if you change the type of the $i$-th bracket, then the resulting bracket sequence becomes <span class="tex-font-style-it">regular</span>.</p>





```input1
6
(((())
```




```input2
6
()()()
```




```input3
1
)
```




```input4
8
)))(((((
```




```output1
3
```




```output2
0
```




```output3
0
```




```output4
0
```


