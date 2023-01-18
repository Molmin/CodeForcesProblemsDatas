## Description

<div><p>You are given a Young diagram. </p><p>Given diagram is a histogram with $n$ columns of lengths $a_1, a_2, \ldots, a_n$ ($a_1 \geq a_2 \geq \ldots \geq a_n \geq 1$).</p><center> <img class="tex-graphics" src="file://fQipX0rn.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Young diagram for $a=[3,2,2,2,1]$.</span> </center><p>Your goal is to find the largest number of non-overlapping dominos that you can draw inside of this histogram, a domino is a $1 \times 2$ or $2 \times 1$ rectangle.</p></div><div class="input-specification"><p>The first line of input contain one integer $n$ ($1 \leq n \leq 300\,000$): the number of columns in the given histogram.</p><p>The next line of input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 300\,000, a_i \geq a_{i+1}$): the lengths of columns.</p></div><div class="output-specification"><p>Output one integer: the largest number of non-overlapping dominos that you can draw inside of the given Young diagram.</p></div>

## Input

<p>The first line of input contain one integer $n$ ($1 \leq n \leq 300\,000$): the number of columns in the given histogram.</p><p>The next line of input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 300\,000, a_i \geq a_{i+1}$): the lengths of columns.</p>

## Output

<p>Output one integer: the largest number of non-overlapping dominos that you can draw inside of the given Young diagram.</p>





```input1
5
3 2 2 2 1
```




```output1
4
```



## Note

<p>Some of the possible solutions for the example:</p><p><img class="tex-graphics" src="file://RkH6W2L2.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://Qo9u1E42.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
