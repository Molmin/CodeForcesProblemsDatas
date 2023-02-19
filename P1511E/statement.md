## Description

<div><p>You have a large rectangular board which is divided into $n \times m$ cells (the board has $n$ rows and $m$ columns). Each cell is either white or black.</p><p>You paint each white cell either red or blue. Obviously, the number of different ways to paint them is $2^w$, where $w$ is the number of white cells.</p><p>After painting the white cells of the board, you want to place the maximum number of dominoes on it, according to the following rules:</p><ul> <li> each domino covers two adjacent cells; </li><li> each cell is covered by at most one domino; </li><li> if a domino is placed horizontally (it covers two adjacent cells in one of the rows), it should cover only red cells; </li><li> if a domino is placed vertically (it covers two adjacent cells in one of the columns), it should cover only blue cells. </li></ul><p>Let the <span class="tex-font-style-it">value</span> of the board be the maximum number of dominoes you can place. Calculate the sum of <span class="tex-font-style-it">values</span> of the board over all $2^w$ possible ways to paint it. Since it can be huge, print it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 3 \cdot 10^5$; $nm \le 3 \cdot 10^5$) — the number of rows and columns, respectively.</p><p>Then $n$ lines follow, each line contains a string of $m$ characters. The $j$-th character in the $i$-th string is <span class="tex-font-style-tt">*</span> if the $j$-th cell in the $i$-th row is black; otherwise, that character is <span class="tex-font-style-tt">o</span>.</p></div><div class="output-specification"><p>Print one integer — the sum of <span class="tex-font-style-it">values</span> of the board over all $2^w$ possible ways to paint it, taken modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 3 \cdot 10^5$; $nm \le 3 \cdot 10^5$) — the number of rows and columns, respectively.</p><p>Then $n$ lines follow, each line contains a string of $m$ characters. The $j$-th character in the $i$-th string is <span class="tex-font-style-tt">*</span> if the $j$-th cell in the $i$-th row is black; otherwise, that character is <span class="tex-font-style-tt">o</span>.</p>

## Output

<p>Print one integer — the sum of <span class="tex-font-style-it">values</span> of the board over all $2^w$ possible ways to paint it, taken modulo $998\,244\,353$.</p>





```input1
3 4
**oo
oo*o
**oo
```




```input2
3 4
**oo
oo**
**oo
```




```input3
2 2
oo
o*
```




```input4
1 4
oooo
```




```output1
144
```




```output2
48
```




```output3
4
```




```output4
9
```


