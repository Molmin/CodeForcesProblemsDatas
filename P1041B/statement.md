## Description

<div><p>Monocarp has decided to buy a new TV set and hang it on the wall in his flat. The wall has enough free space so Monocarp can buy a TV set with screen width not greater than $a$ and screen height not greater than $b$. Monocarp is also used to TV sets with a certain aspect ratio: formally, if the width of the screen is $w$, and the height of the screen is $h$, then the following condition should be met: $\frac{w}{h} = \frac{x}{y}$.</p><p>There are many different TV sets in the shop. Monocarp is sure that for any pair of <span class="tex-font-style-bf">positive integers</span> $w$ and $h$ there is a TV set with screen width $w$ and height $h$ in the shop.</p><p>Monocarp isn't ready to choose the exact TV set he is going to buy. Firstly he wants to determine the optimal screen resolution. He has decided to try all possible variants of screen size. But he must count the number of pairs of <span class="tex-font-style-bf">positive integers</span> $w$ and $h$, beforehand, such that $(w \le a)$, $(h \le b)$ and $(\frac{w}{h} = \frac{x}{y})$.</p><p>In other words, Monocarp wants to determine the number of TV sets having aspect ratio $\frac{x}{y}$, screen width not exceeding $a$, and screen height not exceeding $b$. Two TV sets are considered different if they have different screen width or different screen height.</p></div><div class="input-specification"><p>The first line contains four integers $a$, $b$, $x$, $y$ ($1 \le a, b, x, y \le 10^{18}$)&nbsp;— the constraints on the screen width and height, and on the aspect ratio.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of different variants to choose TV screen width and screen height so that they meet the aforementioned constraints.</p></div>

## Input

<p>The first line contains four integers $a$, $b$, $x$, $y$ ($1 \le a, b, x, y \le 10^{18}$)&nbsp;— the constraints on the screen width and height, and on the aspect ratio.</p>

## Output

<p>Print one integer&nbsp;— the number of different variants to choose TV screen width and screen height so that they meet the aforementioned constraints.</p>





```input1
17 15 5 3

```




```input2
14 16 7 22

```




```input3
4 2 6 4

```




```input4
1000000000000000000 1000000000000000000 999999866000004473 999999822000007597

```




```output1
3

```




```output2
0

```




```output3
1

```




```output4
1000000063

```



## Note

<p>In the first example, there are $3$ possible variants: $(5, 3)$, $(10, 6)$, $(15, 9)$.</p><p>In the second example, there is no TV set meeting the constraints.</p><p>In the third example, there is only one variant: $(3, 2)$.</p>
