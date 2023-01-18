## Description

<div><p>It is the middle of 2018 and Maria Stepanovna, who lives outside Krasnokamensk (a town in Zabaikalsky region), wants to rent three displays to highlight an important problem.</p><p>There are $n$ displays placed along a road, and the $i$-th of them can display a text with font size $s_i$ only. Maria Stepanovna wants to rent such three displays with indices $i &lt; j &lt; k$ that the font size increases if you move along the road in a particular direction. Namely, the condition $s_i &lt; s_j &lt; s_k$ should be held.</p><p>The rent cost is for the $i$-th display is $c_i$. Please determine the smallest cost Maria Stepanovna should pay.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($3 \le n \le 3\,000$)&nbsp;— the number of displays.</p><p>The second line contains $n$ integers $s_1, s_2, \ldots, s_n$ ($1 \le s_i \le 10^9$)&nbsp;— the font sizes on the displays in the order they stand along the road.</p><p>The third line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le 10^8$)&nbsp;— the rent costs for each display.</p></div><div class="output-specification"><p>If there are no three displays that satisfy the criteria, print <span class="tex-font-style-tt">-1</span>. Otherwise print a single integer&nbsp;— the minimum total rent cost of three displays with indices $i &lt; j &lt; k$ such that $s_i &lt; s_j &lt; s_k$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($3 \le n \le 3\,000$)&nbsp;— the number of displays.</p><p>The second line contains $n$ integers $s_1, s_2, \ldots, s_n$ ($1 \le s_i \le 10^9$)&nbsp;— the font sizes on the displays in the order they stand along the road.</p><p>The third line contains $n$ integers $c_1, c_2, \ldots, c_n$ ($1 \le c_i \le 10^8$)&nbsp;— the rent costs for each display.</p>

## Output

<p>If there are no three displays that satisfy the criteria, print <span class="tex-font-style-tt">-1</span>. Otherwise print a single integer&nbsp;— the minimum total rent cost of three displays with indices $i &lt; j &lt; k$ such that $s_i &lt; s_j &lt; s_k$.</p>





```input1
5
2 4 5 4 10
40 30 20 10 40

```




```input2
3
100 101 100
2 4 5

```




```input3
10
1 2 3 4 5 6 7 8 9 10
10 13 11 14 15 12 13 13 18 13

```




```output1
90

```




```output2
-1

```




```output3
33

```



## Note

<p>In the first example you can, for example, choose displays $1$, $4$ and $5$, because $s_1 &lt; s_4 &lt; s_5$ ($2 &lt; 4 &lt; 10$), and the rent cost is $40 + 10 + 40 = 90$.</p><p>In the second example you can't select a valid triple of indices, so the answer is <span class="tex-font-style-tt">-1</span>.</p>
