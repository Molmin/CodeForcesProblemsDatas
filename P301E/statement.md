## Description

<div><p>Yaroslav calls an array of <span class="tex-span"><i>r</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-font-style-it">good</span>, if it meets the following conditions: <span class="tex-span">|<i>a</i><sub class="lower-index">1</sub> - <i>a</i><sub class="lower-index">2</sub>| = 1, |<i>a</i><sub class="lower-index">2</sub> - <i>a</i><sub class="lower-index">3</sub>| = 1, ..., |<i>a</i><sub class="lower-index"><i>r</i> - 1</sub> - <i>a</i><sub class="lower-index"><i>r</i></sub>| = 1, |<i>a</i><sub class="lower-index"><i>r</i></sub> - <i>a</i><sub class="lower-index">1</sub>| = 1</span>, at that <img align="middle" class="tex-formula" src="file://BRa2sAJ8.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>An array of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>r</i></sub></span> is called <span class="tex-font-style-it">great</span>, if it meets the following conditions:</p><ol> <li> The elements in it do not decrease <span class="tex-span">(<i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>. </li><li> If the inequalities <span class="tex-span">1 ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span> hold. </li><li> If we can rearrange its elements and get at least one and at most <span class="tex-span"><i>k</i></span> distinct good arrays. </li></ol><p>Yaroslav has three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span>. He needs to count the number of distinct great arrays. Help Yaroslav! As the answer may be rather large, print the remainder after dividing it by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>Two arrays are considered distinct if there is a position in which they have distinct numbers.</p></div><div class="input-specification"><p>The single line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100)</span>.</p></div><div class="output-specification"><p>In a single line print the remainder after dividing the answer to the problem by number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The single line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 100)</span>.</p>

## Output

<p>In a single line print the remainder after dividing the answer to the problem by number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
1 1 1

```




```input2
3 3 3

```




```output1
0

```




```output2
2

```


