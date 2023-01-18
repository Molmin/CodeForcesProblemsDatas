## Description

<div><p>There are <span class="tex-span"><i>n</i></span> boxes with colored balls on the table. Colors are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. <span class="tex-span"><i>i</i></span>-th box contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> balls, all of which have color <span class="tex-span"><i>i</i></span>. You have to write a program that will divide all balls into sets such that:</p><ul> <li> each ball belongs to exactly one of the sets, </li><li> there are no empty sets, </li><li> there is no set containing two (or more) balls of different colors (each set contains only balls of one color), </li><li> there are no two sets such that the difference between their sizes is greater than <span class="tex-span">1</span>. </li></ul><p>Print the minimum possible number of sets.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print one integer number — the minimum possible number of sets.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print one integer number — the minimum possible number of sets.</p>





```input1
3
4 7 8

```




```input2
2
2 7

```




```output1
5

```




```output2
4

```



## Note

<p>In the first example the balls can be divided into sets like that: one set with <span class="tex-span">4</span> balls of the first color, two sets with <span class="tex-span">3</span> and <span class="tex-span">4</span> balls, respectively, of the second color, and two sets with <span class="tex-span">4</span> balls of the third color.</p>
