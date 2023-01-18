## Description

<div><p>Vadim loves decorating the Christmas tree, so he got a beautiful garland as a present. It consists of $n$ light bulbs in a single row. Each bulb has a number from $1$ to $n$ (in arbitrary order), such that all the numbers are distinct. While Vadim was solving problems, his home Carp removed some light bulbs from the garland. Now Vadim wants to put them back on.</p><center><img class="tex-graphics" src="file://VTfZKR6Y.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Vadim wants to put all bulb back on the garland. Vadim defines <span class="tex-font-style-it">complexity</span> of a garland to be the number of pairs of adjacent bulbs with numbers with different parity (remainder of the division by $2$). For example, the complexity of <span class="tex-font-style-tt">1 4 2 3 5</span> is $2$ and the complexity of <span class="tex-font-style-tt">1 3 5 7 6 4 2</span> is $1$.</p><p>No one likes complexity, so Vadim wants to minimize the number of such pairs. Find the way to put all bulbs back on the garland, such that the complexity is as small as possible.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of light bulbs on the garland.</p><p>The second line contains $n$ integers $p_1,\ p_2,\ \ldots,\ p_n$ ($0 \le p_i \le n$)&nbsp;— the number on the $i$-th bulb, or $0$ if it was removed.</p></div><div class="output-specification"><p>Output a single number&nbsp;— the minimum <span class="tex-font-style-it">complexity</span> of the garland.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the number of light bulbs on the garland.</p><p>The second line contains $n$ integers $p_1,\ p_2,\ \ldots,\ p_n$ ($0 \le p_i \le n$)&nbsp;— the number on the $i$-th bulb, or $0$ if it was removed.</p>

## Output

<p>Output a single number&nbsp;— the minimum <span class="tex-font-style-it">complexity</span> of the garland.</p>





```input1
5
0 5 0 2 3
```




```input2
7
1 0 0 5 0 0 2
```




```output1
2
```




```output2
1
```



## Note

<p>In the first example, one should place light bulbs as <span class="tex-font-style-tt">1 5 4 2 3</span>. In that case, the complexity would be equal to 2, because only $(5, 4)$ and $(2, 3)$ are the pairs of adjacent bulbs that have different parity.</p><p>In the second case, one of the correct answers is <span class="tex-font-style-tt">1 7 3 5 6 4 2</span>. </p>
