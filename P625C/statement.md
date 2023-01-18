## Description

<div><p>People do many crazy things to stand out in a crowd. Some of them dance, some learn by heart rules of Russian language, some try to become an outstanding competitive programmers, while others collect funny math objects.</p><p>Alis is among these collectors. Right now she wants to get one of <span class="tex-span"><i>k</i></span>-special tables. In case you forget, the table <span class="tex-span"><i>n</i> × <i>n</i></span> is called <span class="tex-span"><i>k</i></span>-special if the following three conditions are satisfied:</p><ul> <li> every integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> appears in the table exactly once; </li><li> in each row numbers are situated in increasing order; </li><li> the sum of numbers in the <span class="tex-span"><i>k</i></span>-th column is maximum possible. </li></ul><p>Your goal is to help Alice and find at least one <span class="tex-span"><i>k</i></span>-special table of size <span class="tex-span"><i>n</i> × <i>n</i></span>. Both rows and columns are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, with rows numbered from top to bottom and columns numbered from left to right.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500, 1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the size of the table Alice is looking for and the column that should have maximum possible sum.</p></div><div class="output-specification"><p>First print the sum of the integers in the <span class="tex-span"><i>k</i></span>-th column of the required table.</p><p>Next <span class="tex-span"><i>n</i></span> lines should contain the description of the table itself: first line should contains <span class="tex-span"><i>n</i></span> elements of the first row, second line should contain <span class="tex-span"><i>n</i></span> elements of the second row and so on.</p><p>If there are multiple suitable table, you are allowed to print any.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500, 1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the size of the table Alice is looking for and the column that should have maximum possible sum.</p>

## Output

<p>First print the sum of the integers in the <span class="tex-span"><i>k</i></span>-th column of the required table.</p><p>Next <span class="tex-span"><i>n</i></span> lines should contain the description of the table itself: first line should contains <span class="tex-span"><i>n</i></span> elements of the first row, second line should contain <span class="tex-span"><i>n</i></span> elements of the second row and so on.</p><p>If there are multiple suitable table, you are allowed to print any.</p>





```input1
4 1

```




```input2
5 3

```




```output1
28
1 2 3 4
5 6 7 8
9 10 11 12
13 14 15 16

```




```output2
85
5 6 17 18 19
9 10 23 24 25
7 8 20 21 22
3 4 14 15 16
1 2 11 12 13


```


