## Description

<div><p>Array of integers is <span class="tex-font-style-it">unimodal</span>, if:</p><ul> <li> it is strictly increasing in the beginning; </li><li> after that it is constant; </li><li> after that it is strictly decreasing. </li></ul><p>The first block (increasing) and the last block (decreasing) may be absent. It is allowed that both of this blocks are absent.</p><p>For example, the following three arrays are unimodal: <span class="tex-span">[5, 7, 11, 11, 2, 1]</span>, <span class="tex-span">[4, 4, 2]</span>, <span class="tex-span">[7]</span>, but the following three are not unimodal: <span class="tex-span">[5, 5, 6, 6, 1]</span>, <span class="tex-span">[1, 2, 1, 2]</span>, <span class="tex-span">[4, 5, 5, 6]</span>.</p><p>Write a program that checks if an array is unimodal.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000</span>) — the elements of the array.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if the given array is unimodal. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can output each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements in the array.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000</span>) — the elements of the array.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if the given array is unimodal. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p><p>You can output each letter in any case (upper or lower).</p>





```input1
6
1 5 5 5 4 2

```




```input2
5
10 20 30 20 10

```




```input3
4
1 2 1 2

```




```input4
7
3 3 3 3 3 3 3

```




```output1
YES

```




```output2
YES

```




```output3
NO

```




```output4
YES

```



## Note

<p>In the first example the array is unimodal, because it is strictly increasing in the beginning (from position <span class="tex-span">1</span> to position <span class="tex-span">2</span>, inclusively), that it is constant (from position <span class="tex-span">2</span> to position <span class="tex-span">4</span>, inclusively) and then it is strictly decreasing (from position <span class="tex-span">4</span> to position <span class="tex-span">6</span>, inclusively).</p>
