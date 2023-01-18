## Description

<div><p>Petya's friends made him a birthday present — a bracket sequence. Petya was quite disappointed with his gift, because he dreamed of correct bracket sequence, yet he told his friends nothing about his dreams and decided to fix present himself. </p><p>To make everything right, Petya is going to move at most one bracket from its original place in the sequence to any other position. Reversing the bracket (e.g. turning "(" into ")" or vice versa) isn't allowed. </p><p>We remind that bracket sequence $s$ is called correct if: </p><ul> <li> $s$ is empty; </li><li> $s$ is equal to "<span class="tex-font-style-tt">(</span>$t$<span class="tex-font-style-tt">)</span>", where $t$ is correct bracket sequence; </li><li> $s$ is equal to $t_1 t_2$, i.e. concatenation of $t_1$ and $t_2$, where $t_1$ and $t_2$ are correct bracket sequences. </li></ul><p>For example, "<span class="tex-font-style-tt">(()())</span>", "<span class="tex-font-style-tt">()</span>" are correct, while "<span class="tex-font-style-tt">)(</span>" and "<span class="tex-font-style-tt">())</span>" are not. Help Petya to fix his birthday present and understand whether he can move one bracket so that the sequence becomes correct.</p></div><div class="input-specification"><p>First of line of input contains a single number $n$ ($1 \leq n \leq 200\,000$)&nbsp;— length of the sequence which Petya received for his birthday.</p><p>Second line of the input contains bracket sequence of length $n$, containing symbols "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if Petya can make his sequence correct moving at most one bracket. Otherwise print "<span class="tex-font-style-tt">No</span>".</p></div>

## Input

<p>First of line of input contains a single number $n$ ($1 \leq n \leq 200\,000$)&nbsp;— length of the sequence which Petya received for his birthday.</p><p>Second line of the input contains bracket sequence of length $n$, containing symbols "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if Petya can make his sequence correct moving at most one bracket. Otherwise print "<span class="tex-font-style-tt">No</span>".</p>





```input1
2
)(
```




```input2
3
(()
```




```input3
2
()
```




```input4
10
)))))(((((
```




```output1
Yes
```




```output2
No
```




```output3
Yes
```




```output4
No
```



## Note

<p>In the first example, Petya can move first bracket to the end, thus turning the sequence into "<span class="tex-font-style-tt">()</span>", which is correct bracket sequence.</p><p>In the second example, there is no way to move at most one bracket so that the sequence becomes correct.</p><p>In the third example, the sequence is already correct and there's no need to move brackets.</p>
