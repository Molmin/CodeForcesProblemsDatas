## Description

<div><p>Yaroslav has an array that consists of <span class="tex-span"><i>n</i></span> integers. In one second Yaroslav can swap two neighboring array elements. Now Yaroslav is wondering if he can obtain an array where any two neighboring elements would be distinct in a finite time.</p><p>Help Yaroslav.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of elements in the array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the array elements.</p></div><div class="output-specification"><p>In the single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if Yaroslav can obtain the array he needs, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of elements in the array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the array elements.</p>

## Output

<p>In the single line print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if Yaroslav can obtain the array he needs, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
1
1

```




```input2
3
1 1 2

```




```input3
4
7 7 7 7

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



## Note

<p>In the first sample the initial array fits well.</p><p>In the second sample Yaroslav can get array: <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span>. He can swap the last and the second last elements to obtain it.</p><p>In the third sample Yarosav can't get the array he needs.</p><p> </p><p> </p><p> </p><p> </p><p> </p><p> </p>
