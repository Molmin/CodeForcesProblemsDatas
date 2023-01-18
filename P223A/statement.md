## Description

<div><p>A <span class="tex-font-style-it">bracket sequence</span> is a string, containing only characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>", "<span class="tex-font-style-tt">[</span>" and "<span class="tex-font-style-tt">]</span>".</p><p>A <span class="tex-font-style-it">correct bracket sequence</span> is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example, bracket sequences "<span class="tex-font-style-tt">()[]</span>", "<span class="tex-font-style-tt">([])</span>" are correct (the resulting expressions are: "<span class="tex-font-style-tt">(1)+[1]</span>", "<span class="tex-font-style-tt">([1+1]+1)</span>"), and "<span class="tex-font-style-tt">](</span>" and "<span class="tex-font-style-tt">[</span>" are not. <span class="tex-font-style-bf">The empty string is a correct bracket sequence by definition.</span></p><p>A <span class="tex-font-style-it">substring</span> <span class="tex-span"><i>s</i>[<i>l</i>... <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|)</span> of string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>) is the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>s</i><sub class="lower-index"><i>r</i></sub></span>. <span class="tex-font-style-bf">The empty string is a substring of any string by definition</span>.</p><p>You are given a bracket sequence, not necessarily correct. Find its substring which is a correct bracket sequence and contains as many opening square brackets «<span class="tex-font-style-tt">[</span>» as possible.</p></div><div class="input-specification"><p>The first and the only line contains the bracket sequence as a string, consisting only of characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>", "<span class="tex-font-style-tt">[</span>" and "<span class="tex-font-style-tt">]</span>". It is guaranteed that the string is non-empty and its length doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p></div><div class="output-specification"><p>In the first line print a single integer — the number of brackets «<span class="tex-font-style-tt">[</span>» in the required bracket sequence. In the second line print the optimal sequence. If there are more than one optimal solutions print any of them.</p></div>

## Input

<p>The first and the only line contains the bracket sequence as a string, consisting only of characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>", "<span class="tex-font-style-tt">[</span>" and "<span class="tex-font-style-tt">]</span>". It is guaranteed that the string is non-empty and its length doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p>

## Output

<p>In the first line print a single integer — the number of brackets «<span class="tex-font-style-tt">[</span>» in the required bracket sequence. In the second line print the optimal sequence. If there are more than one optimal solutions print any of them.</p>





```input1
([])

```




```input2
(((

```




```output1
1
([])

```




```output2
0


```


