## Description

<div><p>One spring day on his way to university Lesha found an array <span class="tex-span"><i>A</i></span>. Lesha likes to split arrays into several parts. This time Lesha decided to split the array <span class="tex-span"><i>A</i></span> into several, possibly one, new arrays so that the sum of elements in each of the new arrays is not zero. One more condition is that if we place the new arrays one after another they will form the old array <span class="tex-span"><i>A</i></span>.</p><p>Lesha is tired now so he asked you to split the array. Help Lesha!</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of elements in the array <span class="tex-span"><i>A</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">3</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the elements of the array <span class="tex-span"><i>A</i></span>.</p></div><div class="output-specification"><p>If it is not possible to split the array <span class="tex-span"><i>A</i></span> and satisfy all the constraints, print single line containing "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes). In the next line print single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of new arrays. In each of the next <span class="tex-span"><i>k</i></span> lines print two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> which denote the subarray <span class="tex-span"><i>A</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>... <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> of the initial array <span class="tex-span"><i>A</i></span> being the <span class="tex-span"><i>i</i></span>-th new array. Integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> should satisfy the following conditions:</p><ul> <li> <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> = 1</span> </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub> = <i>n</i></span> </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> + 1 = <i>l</i><sub class="lower-index"><i>i</i> + 1</sub></span> for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>. </li></ul><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of elements in the array <span class="tex-span"><i>A</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">3</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the elements of the array <span class="tex-span"><i>A</i></span>.</p>

## Output

<p>If it is not possible to split the array <span class="tex-span"><i>A</i></span> and satisfy all the constraints, print single line containing "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise in the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes). In the next line print single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of new arrays. In each of the next <span class="tex-span"><i>k</i></span> lines print two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> which denote the subarray <span class="tex-span"><i>A</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>... <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> of the initial array <span class="tex-span"><i>A</i></span> being the <span class="tex-span"><i>i</i></span>-th new array. Integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> should satisfy the following conditions:</p><ul> <li> <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> = 1</span> </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub> = <i>n</i></span> </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> + 1 = <i>l</i><sub class="lower-index"><i>i</i> + 1</sub></span> for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>. </li></ul><p>If there are multiple answers, print any of them.</p>





```input1
3
1 2 -3

```




```input2
8
9 -12 3 4 -4 -10 7 3

```




```input3
1
0

```




```input4
4
1 2 3 -5

```




```output1
YES
2
1 2
3 3

```




```output2
YES
2
1 2
3 8

```




```output3
NO

```




```output4
YES
4
1 1
2 2
3 3
4 4

```


