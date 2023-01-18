## Description

<div><p>Rainbow built <span class="tex-span"><i>h</i></span> cells in a row that are numbered from 1 to <span class="tex-span"><i>h</i></span> from left to right. There are <span class="tex-span"><i>n</i></span> cells with treasure. We call each of these <span class="tex-span"><i>n</i></span> cells "Treasure Cell". The <span class="tex-span"><i>i</i></span>-th "Treasure Cell" is the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th cell and the value of treasure in it is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> dollars.</p><p>Then, Freda went in the first cell. For now, she can go just <span class="tex-span"><i>k</i></span> cells forward, or return to the first cell. That means Freda was able to reach the 1st, (<span class="tex-span"><i>k</i> + 1</span>)-th, (<span class="tex-span">2·<i>k</i> + 1</span>)-th, (<span class="tex-span">3·<i>k</i> + 1</span>)-th cells and so on.</p><p>Then Rainbow gave Freda <span class="tex-span"><i>m</i></span> operations. Each operation is one of the following three types:</p><ol> <li> Add another method <span class="tex-span"><i>x</i></span>: she can also go just <span class="tex-span"><i>x</i></span> cells forward at any moment. For example, initially she has only one method <span class="tex-span"><i>k</i></span>. If at some moment she has methods <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> then she can reach all the cells with number in form <img align="middle" class="tex-formula" src="file://4o1SrIOe.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> — some non-negative integer. </li><li> Reduce the value of the treasure in the <span class="tex-span"><i>x</i></span>-th "Treasure Cell" by <span class="tex-span"><i>y</i></span> dollars. In other words, to apply assignment <span class="tex-span"><i>c</i><sub class="lower-index"><i>x</i></sub> = <i>c</i><sub class="lower-index"><i>x</i></sub> - <i>y</i></span>. </li><li> Ask the value of the most valuable treasure among the cells Freda can reach. If Freda cannot reach any cell with the treasure then consider the value of the most valuable treasure equal to 0, and do nothing. Otherwise take the most valuable treasure away. If several "Treasure Cells" have the most valuable treasure, take the "Treasure Cell" with the minimum number (not necessarily with the minimum number of cell). After that the total number of cells with a treasure is decreased by one. </li></ol><p>As a programmer, you are asked by Freda to write a program to answer each query.</p></div><div class="input-specification"><p>The first line of the input contains four integers: <span class="tex-span"><i>h</i>&nbsp;(1 ≤ <i>h</i> ≤ 10<sup class="upper-index">18</sup>), <i>n</i>, <i>m</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> and <span class="tex-span"><i>k</i>&nbsp;(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i>), <i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. That means the <span class="tex-span"><i>i</i></span>-th "Treasure Cell" is the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th cell and cost of the treasure in that cell is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> dollars. All the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines is in one of the three following formats:</p><ul> <li> "1 <span class="tex-span"><i>x</i></span>" — an operation of type 1, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>h</i></span>; </li><li> "2 <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" — an operation of type 2, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 0 ≤ <i>y</i> &lt; <i>c</i><sub class="lower-index"><i>x</i></sub></span>; </li><li> "3" — an operation of type 3. </li></ul><p>There are at most 20 operations of type 1. It's guaranteed that at any moment treasure in each cell has positive value. It's guaranteed that all operations is correct (no operation can decrease the value of the taken tresure).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>For each operation of type 3, output an integer indicates the value (in dollars) of the most valuable treasure among the "Treasure Cells" Freda can reach. If there is no such treasure, output 0.</p></div>

## Input

<p>The first line of the input contains four integers: <span class="tex-span"><i>h</i>&nbsp;(1 ≤ <i>h</i> ≤ 10<sup class="upper-index">18</sup>), <i>n</i>, <i>m</i>&nbsp;(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> and <span class="tex-span"><i>k</i>&nbsp;(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>h</i>), <i>c</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. That means the <span class="tex-span"><i>i</i></span>-th "Treasure Cell" is the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th cell and cost of the treasure in that cell is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> dollars. All the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines is in one of the three following formats:</p><ul> <li> "1 <span class="tex-span"><i>x</i></span>" — an operation of type 1, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>h</i></span>; </li><li> "2 <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span>" — an operation of type 2, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 0 ≤ <i>y</i> &lt; <i>c</i><sub class="lower-index"><i>x</i></sub></span>; </li><li> "3" — an operation of type 3. </li></ul><p>There are at most 20 operations of type 1. It's guaranteed that at any moment treasure in each cell has positive value. It's guaranteed that all operations is correct (no operation can decrease the value of the taken tresure).</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>For each operation of type 3, output an integer indicates the value (in dollars) of the most valuable treasure among the "Treasure Cells" Freda can reach. If there is no such treasure, output 0.</p>





```input1
10 3 5 2
5 50
7 60
8 100
2 2 5
3
1 3
3
3

```




```output1
55
100
50

```



## Note

<p>In the sample, there are 10 cells and 3 "Treasure Cells". The first "Treasure Cell" is cell 5, having 50 dollars tresure in it. The second "Treasure Cell" is cell 7, having 60 dollars tresure in it. The third "Treasure Cell" is cell 8, having 100 dollars tresure in it.</p><p>At first, Freda can only reach cell 1, 3, 5, 7 and 9. In the first operation, we reduce the value in the second "Treasure Cell" from 60 to 55. Then the most valuable treasure among the "Treasure Cells" she can reach is max(50, 55) = 55. After the third operation, she can also go 3 cells forward each step, being able to reach cell 1, 3, 4, 5, 6, 7, 8, 9, 10. So the most valuable tresure is 100.</p><p>Noticed that she took the 55 dollars and 100 dollars treasure away, so the last answer is 50.</p>
