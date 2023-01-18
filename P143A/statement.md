## Description

<div><p>Vasilisa the Wise from the Kingdom of Far Far Away got a magic box with a secret as a present from her friend Hellawisa the Wise from the Kingdom of A Little Closer. However, Vasilisa the Wise does not know what the box's secret is, since she cannot open it again. She hopes that you will help her one more time with that.</p><p>The box's lock looks as follows: it contains <span class="tex-span">4</span> identical deepenings for gems as a <span class="tex-span">2 × 2</span> square, and some integer numbers are written at the lock's edge near the deepenings. The example of a lock is given on the picture below.</p><center> <img class="tex-graphics" src="file://X2Aa1EzJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The box is accompanied with <span class="tex-span">9</span> gems. Their shapes match the deepenings' shapes and each gem contains one number from <span class="tex-span">1</span> to <span class="tex-span">9</span> (each number is written on exactly one gem). The box will only open after it is decorated with gems correctly: that is, each deepening in the lock should be filled with exactly one gem. Also, the sums of numbers in the square's rows, columns and two diagonals of the square should match the numbers written at the lock's edge. For example, the above lock will open if we fill the deepenings with gems with numbers as is shown on the picture below.</p><center> <img class="tex-graphics" src="file://TP9uH1Xj.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Now Vasilisa the Wise wants to define, given the numbers on the box's lock, which gems she should put in the deepenings to open the box. Help Vasilisa to solve this challenging task.</p></div><div class="input-specification"><p>The input contains numbers written on the edges of the lock of the box. The first line contains space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> that define the required sums of numbers in the rows of the square. The second line contains space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> that define the required sums of numbers in the columns of the square. The third line contains space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span> that define the required sums of numbers on the main and on the side diagonals of the square (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub> ≤ 20</span>). Correspondence between the above 6 variables and places where they are written is shown on the picture below. For more clarifications please look at the second sample test that demonstrates the example given in the problem statement.</p><center> <img class="tex-graphics" src="file://rKTlSz21.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="output-specification"><p>Print the scheme of decorating the box with stones: two lines containing two space-separated integers from <span class="tex-span">1</span> to <span class="tex-span">9</span>. The numbers should be pairwise different. If there is no solution for the given lock, then print the single number "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>If there are several solutions, output any.</p></div>

## Input

<p>The input contains numbers written on the edges of the lock of the box. The first line contains space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> that define the required sums of numbers in the rows of the square. The second line contains space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> that define the required sums of numbers in the columns of the square. The third line contains space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index">2</sub></span> that define the required sums of numbers on the main and on the side diagonals of the square (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>d</i><sub class="lower-index">1</sub>, <i>d</i><sub class="lower-index">2</sub> ≤ 20</span>). Correspondence between the above 6 variables and places where they are written is shown on the picture below. For more clarifications please look at the second sample test that demonstrates the example given in the problem statement.</p><center> <img class="tex-graphics" src="file://rKTlSz21.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>

## Output

<p>Print the scheme of decorating the box with stones: two lines containing two space-separated integers from <span class="tex-span">1</span> to <span class="tex-span">9</span>. The numbers should be pairwise different. If there is no solution for the given lock, then print the single number "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p><p>If there are several solutions, output any.</p>





```input1
3 7
4 6
5 5

```




```input2
11 10
13 8
5 16

```




```input3
1 2
3 4
5 6

```




```input4
10 10
10 10
10 10

```




```output1
1 2
3 4

```




```output2
4 7
9 1

```




```output3
-1

```




```output4
-1

```



## Note

<p>Pay attention to the last test from the statement: it is impossible to open the box because for that Vasilisa the Wise would need 4 identical gems containing number "5". However, Vasilisa only has one gem with each number from <span class="tex-span">1</span> to <span class="tex-span">9</span>.</p>
