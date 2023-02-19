## Description

<div><p>Vasya has a sequence of cubes and exactly one integer is written on each cube. Vasya exhibited all his cubes in a row. So the sequence of numbers written on the cubes in the order from the left to the right equals to <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>While Vasya was walking, his little brother Stepan played with Vasya's cubes and changed their order, so now the sequence of numbers written on the cubes became equal to <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>Stepan said that he swapped only cubes which where on the positions between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, inclusive, and did not remove or add any other cubes (i. e. he said that he reordered cubes between positions <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, inclusive, in some way).</p><p>Your task is to determine if it is possible that Stepan said the truth, or it is guaranteed that Stepan deceived his brother.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) — the number of Vasya's cubes and the positions told by Stepan.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of integers written on cubes in the Vasya's order.</p><p>The third line contains the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of integers written on cubes after Stepan rearranged their order.</p><p>It is guaranteed that Stepan did not remove or add other cubes, he only rearranged Vasya's cubes.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">LIE</span>" (without quotes) if it is guaranteed that Stepan deceived his brother. In the other case, print "<span class="tex-font-style-tt">TRUTH</span>" (without quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) — the number of Vasya's cubes and the positions told by Stepan.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of integers written on cubes in the Vasya's order.</p><p>The third line contains the sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the sequence of integers written on cubes after Stepan rearranged their order.</p><p>It is guaranteed that Stepan did not remove or add other cubes, he only rearranged Vasya's cubes.</p>

## Output

<p>Print "<span class="tex-font-style-tt">LIE</span>" (without quotes) if it is guaranteed that Stepan deceived his brother. In the other case, print "<span class="tex-font-style-tt">TRUTH</span>" (without quotes).</p>





```input1
5 2 4
3 4 2 3 1
3 2 3 4 1

```




```input2
3 1 2
1 2 3
3 1 2

```




```input3
4 2 4
1 1 1 1
1 1 1 1

```




```output1
TRUTH

```




```output2
LIE

```




```output3
TRUTH

```



## Note

<p>In the first example there is a situation when Stepan said the truth. Initially the sequence of integers on the cubes was equal to <span class="tex-font-style-tt">[3, 4, 2, 3, 1]</span>. Stepan could at first swap cubes on positions <span class="tex-span">2</span> and <span class="tex-span">3</span> (after that the sequence of integers on cubes became equal to <span class="tex-font-style-tt">[3, 2, 4, 3, 1]</span>), and then swap cubes in positions <span class="tex-span">3</span> and <span class="tex-span">4</span> (after that the sequence of integers on cubes became equal to <span class="tex-font-style-tt">[3, 2, 3, 4, 1]</span>).</p><p>In the second example it is not possible that Stepan said truth because he said that he swapped cubes only between positions <span class="tex-span">1</span> and <span class="tex-span">2</span>, but we can see that it is guaranteed that he changed the position of the cube which was on the position <span class="tex-span">3</span> at first. So it is guaranteed that Stepan deceived his brother.</p><p>In the third example for any values <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> there is a situation when Stepan said the truth.</p>
