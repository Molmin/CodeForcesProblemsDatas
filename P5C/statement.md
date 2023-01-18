## Description

<div><p>This is yet another problem dealing with regular bracket sequences.</p><p>We should remind you that a bracket sequence is called regular, if by inserting «<span class="tex-font-style-tt">+</span>» and «<span class="tex-font-style-tt">1</span>» into it we can get a correct mathematical expression. For example, sequences «<span class="tex-font-style-tt">(())()</span>», «<span class="tex-font-style-tt">()</span>» and «<span class="tex-font-style-tt">(()(()))</span>» are regular, while «<span class="tex-font-style-tt">)(</span>», «<span class="tex-font-style-tt">(()</span>» and «<span class="tex-font-style-tt">(()))(</span>» are not. </p><p>You are given a string of «<span class="tex-font-style-tt">(</span>» and «<span class="tex-font-style-tt">)</span>» characters. You are to find its longest substring that is a regular bracket sequence. You are to find the number of such substrings as well.</p></div><div class="input-specification"><p>The first line of the input file contains a non-empty string, consisting of «<span class="tex-font-style-tt">(</span>» and «<span class="tex-font-style-tt">)</span>» characters. Its length does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print the length of the longest substring that is a regular bracket sequence, and the number of such substrings. If there are no such substrings, write the only line containing "<span class="tex-font-style-tt">0 1</span>".</p></div>

## Input

<p>The first line of the input file contains a non-empty string, consisting of «<span class="tex-font-style-tt">(</span>» and «<span class="tex-font-style-tt">)</span>» characters. Its length does not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print the length of the longest substring that is a regular bracket sequence, and the number of such substrings. If there are no such substrings, write the only line containing "<span class="tex-font-style-tt">0 1</span>".</p>





```input1
)((())))(()())

```




```input2
))(

```




```output1
6 2

```




```output2
0 1

```


