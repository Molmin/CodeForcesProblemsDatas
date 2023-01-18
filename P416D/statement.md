## Description

<div><p>Polycarpus develops an interesting theory about the interrelation of arithmetic progressions with just everything in the world. His current idea is that the population of the capital of Berland changes over time like an arithmetic progression. Well, or like multiple arithmetic progressions.</p><p>Polycarpus believes that if he writes out the population of the capital for several consecutive years in the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, then it is convenient to consider the array as several arithmetic progressions, written one after the other. For example, sequence <span class="tex-span">(8, 6, 4, 2, 1, 4, 7, 10, 2)</span> can be considered as a sequence of three arithmetic progressions <span class="tex-span">(8, 6, 4, 2)</span>, <span class="tex-span">(1, 4, 7, 10)</span> and <span class="tex-span">(2)</span>, which are written one after another.</p><p>Unfortunately, Polycarpus may not have all the data for the <span class="tex-span"><i>n</i></span> consecutive years (a census of the population doesn't occur every year, after all). For this reason, some values of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> ​​may be unknown. Such values are represented by number <span class="tex-font-style-tt">-1</span>.</p><p>For a given sequence <span class="tex-span"><i>a</i> = (<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>)</span>, which consists of positive integers and values ​​<span class="tex-font-style-tt">-1</span>, find the minimum number of arithmetic progressions Polycarpus needs to get <span class="tex-span"><i>a</i></span>. To get <span class="tex-span"><i>a</i></span>, the progressions need to be written down one after the other. Values ​​<span class="tex-font-style-tt">-1</span> may correspond to an arbitrary positive integer and the values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> must be equal to the corresponding elements of sought consecutive record of the progressions.</p><p>Let us remind you that a finite sequence <span class="tex-span"><i>c</i></span> is called an arithmetic progression if the difference <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>c</i><sub class="lower-index"><i>i</i></sub></span> of any two consecutive elements in it is constant. By definition, any sequence of length 1 is an arithmetic progression.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in the sequence. The second line contains integer values <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> separated by a space (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> =  - 1</span>).</p></div><div class="output-specification"><p>Print the minimum number of arithmetic progressions that you need to write one after another to get sequence <span class="tex-span"><i>a</i></span>. The positions marked as <span class="tex-font-style-tt">-1</span> in <span class="tex-span"><i>a</i></span> can be represented by any positive integers.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of elements in the sequence. The second line contains integer values <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> separated by a space (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> or <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> =  - 1</span>).</p>

## Output

<p>Print the minimum number of arithmetic progressions that you need to write one after another to get sequence <span class="tex-span"><i>a</i></span>. The positions marked as <span class="tex-font-style-tt">-1</span> in <span class="tex-span"><i>a</i></span> can be represented by any positive integers.</p>





```input1
9
8 6 4 2 1 4 7 10 2

```




```input2
9
-1 6 -1 2 -1 4 7 -1 2

```




```input3
5
-1 -1 -1 -1 -1

```




```input4
7
-1 -1 4 5 1 2 3

```




```output1
3

```




```output2
3

```




```output3
1

```




```output4
2

```


