## Description

<div><p>There is a square matrix <span class="tex-span"><i>n</i> × <i>n</i></span>, consisting of non-negative integer numbers. You should find such a way on it that </p><ul> <li> starts in the upper left cell of the matrix; </li><li> each following cell is to the right or down from the current cell; </li><li> the way ends in the bottom right cell. </li></ul><p>Moreover, if we multiply together all the numbers along the way, the result should be the least "round". In other words, it should end in the least possible number of zeros.</p></div><div class="input-specification"><p>The first line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>), <span class="tex-span"><i>n</i></span> is the size of the matrix. Then follow <span class="tex-span"><i>n</i></span> lines containing the matrix elements (non-negative integer numbers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>In the first line print the least number of trailing zeros. In the second line print the correspondent way itself.</p></div>

## Input

<p>The first line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>), <span class="tex-span"><i>n</i></span> is the size of the matrix. Then follow <span class="tex-span"><i>n</i></span> lines containing the matrix elements (non-negative integer numbers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>In the first line print the least number of trailing zeros. In the second line print the correspondent way itself.</p>





```input1
3
1 2 3
4 5 6
7 8 9

```




```output1
0
DDRR

```


