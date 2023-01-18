## Description

<div><p>Vasya studies positional numeral systems. Unfortunately, he often forgets to write the base of notation in which the expression is written. Once he saw a note in his notebook saying <span class="tex-span"><i>a</i> + <i>b</i> = ?</span>, and that the base of the positional notation wasn’t written anywhere. Now Vasya has to choose a base <span class="tex-span"><i>p</i></span> and regard the expression as written in the base <span class="tex-span"><i>p</i></span> positional notation. Vasya understood that he can get different results with different bases, and some bases are even invalid. For example, expression <span class="tex-span">78 + 87</span> in the base 16 positional notation is equal to <span class="tex-span"><i>FF</i><sub class="lower-index">16</sub></span>, in the base 15 positional notation it is equal to <span class="tex-span">110<sub class="lower-index">15</sub></span>, in the base 10 one — to <span class="tex-span">165<sub class="lower-index">10</sub></span>, in the base 9 one — to <span class="tex-span">176<sub class="lower-index">9</sub></span>, and in the base 8 or lesser-based positional notations the expression is invalid as all the numbers should be strictly less than the positional notation base. Vasya got interested in what is the length of the longest possible expression value. Help him to find this length.</p><p>The length of a number should be understood as the number of numeric characters in it. For example, the length of the longest answer for <span class="tex-span">78 + 87 = ?</span> is 3. It is calculated like that in the base 15 (<span class="tex-span">110<sub class="lower-index">15</sub></span>), base 10 (<span class="tex-span">165<sub class="lower-index">10</sub></span>), base 9 (<span class="tex-span">176<sub class="lower-index">9</sub></span>) positional notations, for example, and in some other ones.</p></div><div class="input-specification"><p>The first letter contains two space-separated numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 1000</span>) which represent the given summands.</p></div><div class="output-specification"><p>Print a single number — the length of the longest answer.</p></div>

## Input

<p>The first letter contains two space-separated numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 1000</span>) which represent the given summands.</p>

## Output

<p>Print a single number — the length of the longest answer.</p>





```input1
78 87

```




```input2
1 1

```




```output1
3

```




```output2
2

```


