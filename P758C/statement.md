## Description

<div><p>On the Literature lesson Sergei noticed an awful injustice, it seems that some students are asked more often than others.</p><p>Seating in the class looks like a rectangle, where <span class="tex-span"><i>n</i></span> rows with <span class="tex-span"><i>m</i></span> pupils in each. </p><p>The teacher asks pupils in the following order: at first, she asks all pupils from the first row in the order of their seating, then she continues to ask pupils from the next row. If the teacher asked the last row, then the direction of the poll changes, it means that she asks the previous row. The order of asking the rows looks as follows: the <span class="tex-span">1</span>-st row, the <span class="tex-span">2</span>-nd row, <span class="tex-span">...</span>, the <span class="tex-span"><i>n</i> - 1</span>-st row, the <span class="tex-span"><i>n</i></span>-th row, the <span class="tex-span"><i>n</i> - 1</span>-st row, <span class="tex-span">...</span>, the <span class="tex-span">2</span>-nd row, the <span class="tex-span">1</span>-st row, the <span class="tex-span">2</span>-nd row, <span class="tex-span">...</span></p><p>The order of asking of pupils on the same row is always the same: the <span class="tex-span">1</span>-st pupil, the <span class="tex-span">2</span>-nd pupil, <span class="tex-span">...</span>, the <span class="tex-span"><i>m</i></span>-th pupil.</p><p>During the lesson the teacher managed to ask exactly <span class="tex-span"><i>k</i></span> questions from pupils in order described above. Sergei seats on the <span class="tex-span"><i>x</i></span>-th row, on the <span class="tex-span"><i>y</i></span>-th place in the row. Sergei decided to prove to the teacher that pupils are asked irregularly, help him count three values:</p><ol> <li> the maximum number of questions a particular pupil is asked, </li><li> the minimum number of questions a particular pupil is asked, </li><li> how many times the teacher asked Sergei. </li></ol><p>If there is only one row in the class, then the teacher always asks children from this row.</p></div><div class="input-specification"><p>The first and the only line contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>).</p></div><div class="output-specification"><p>Print three integers:</p><ol> <li> the maximum number of questions a particular pupil is asked, </li><li> the minimum number of questions a particular pupil is asked, </li><li> how many times the teacher asked Sergei. </li></ol></div>

## Input

<p>The first and the only line contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>).</p>

## Output

<p>Print three integers:</p><ol> <li> the maximum number of questions a particular pupil is asked, </li><li> the minimum number of questions a particular pupil is asked, </li><li> how many times the teacher asked Sergei. </li></ol>





```input1
1 3 8 1 1

```




```input2
4 2 9 4 2

```




```input3
5 5 25 4 3

```




```input4
100 100 1000000000000000000 100 100

```




```output1
3 2 3
```




```output2
2 1 1
```




```output3
1 1 1
```




```output4
101010101010101 50505050505051 50505050505051
```



## Note

<p>The order of asking pupils in the first test: </p><ol> <li> the pupil from the first row who seats at the first table, it means it is Sergei; </li><li> the pupil from the first row who seats at the second table; </li><li> the pupil from the first row who seats at the third table; </li><li> the pupil from the first row who seats at the first table, it means it is Sergei; </li><li> the pupil from the first row who seats at the second table; </li><li> the pupil from the first row who seats at the third table; </li><li> the pupil from the first row who seats at the first table, it means it is Sergei; </li><li> the pupil from the first row who seats at the second table; </li></ol><p>The order of asking pupils in the second test: </p><ol> <li> the pupil from the first row who seats at the first table; </li><li> the pupil from the first row who seats at the second table; </li><li> the pupil from the second row who seats at the first table; </li><li> the pupil from the second row who seats at the second table; </li><li> the pupil from the third row who seats at the first table; </li><li> the pupil from the third row who seats at the second table; </li><li> the pupil from the fourth row who seats at the first table; </li><li> the pupil from the fourth row who seats at the second table, it means it is Sergei; </li><li> the pupil from the third row who seats at the first table; </li></ol>
