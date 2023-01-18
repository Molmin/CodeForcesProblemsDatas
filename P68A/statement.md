## Description

<div><p>Little Petya was given this problem for homework:</p><p>You are given function <img align="middle" class="tex-formula" src="file://lpu4yNZo.png" style="max-width: 100.0%;max-height: 100.0%;"> (here <img align="middle" class="tex-formula" src="file://34YOmf0R.png" style="max-width: 100.0%;max-height: 100.0%;"> represents the operation of taking the remainder). His task is to count the number of integers <span class="tex-span"><i>x</i></span> in range <span class="tex-span">[<i>a</i>;<i>b</i>]</span> with property <span class="tex-span"><i>f</i>(<i>x</i>) = <i>x</i></span>.</p><p>It is a pity that Petya forgot the order in which the remainders should be taken and wrote down only 4 numbers. Each of 24 possible orders of taking the remainder has equal probability of being chosen. For example, if Petya has numbers 1, 2, 3, 4 then he can take remainders in that order or first take remainder modulo 4, then modulo 2, 3, 1. There also are 22 other permutations of these numbers that represent orders in which remainder can be taken. In this problem 4 numbers wrote down by Petya will be pairwise distinct.</p><p>Now it is impossible for Petya to complete the task given by teacher but just for fun he decided to find the number of integers <img align="middle" class="tex-formula" src="file://VRL5WJ4z.png" style="max-width: 100.0%;max-height: 100.0%;"> with property that probability that <span class="tex-span"><i>f</i>(<i>x</i>) = <i>x</i></span> is not less than <span class="tex-span">31.4159265352718281828459045%</span>. In other words, Petya will pick up the number <span class="tex-span"><i>x</i></span> if there exist at least <span class="tex-span">7</span> permutations of numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub></span>, for which <span class="tex-span"><i>f</i>(<i>x</i>) = <i>x</i></span>.</p></div><div class="input-specification"><p>First line of the input will contain 6 integers, separated by spaces: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub>, <i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub> ≤ 1000, 0 ≤ <i>a</i> ≤ <i>b</i> ≤ 31415</span>). </p><p>It is guaranteed that numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub></span> will be pairwise distinct.</p></div><div class="output-specification"><p>Output the number of integers in the given range that have the given property.</p></div>

## Input

<p>First line of the input will contain 6 integers, separated by spaces: <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub>, <i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub> ≤ 1000, 0 ≤ <i>a</i> ≤ <i>b</i> ≤ 31415</span>). </p><p>It is guaranteed that numbers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub></span> will be pairwise distinct.</p>

## Output

<p>Output the number of integers in the given range that have the given property.</p>





```input1
2 7 1 8 2 8

```




```input2
20 30 40 50 0 100

```




```input3
31 41 59 26 17 43

```




```output1
0

```




```output2
20

```




```output3
9

```


