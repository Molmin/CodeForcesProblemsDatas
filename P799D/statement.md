## Description

<div><p>In one of the games Arkady is fond of the game process happens on a rectangular field. In the game process Arkady can buy extensions for his field, each extension enlarges one of the field sizes in a particular number of times. Formally, there are <span class="tex-span"><i>n</i></span> extensions, the <span class="tex-span"><i>i</i></span>-th of them multiplies the width or the length (by Arkady's choice) by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Each extension can't be used more than once, the extensions can be used in any order.</p><p>Now Arkady's field has size <span class="tex-span"><i>h</i> × <i>w</i></span>. He wants to enlarge it so that it is possible to place a rectangle of size <span class="tex-span"><i>a</i> × <i>b</i></span> on it (along the width or along the length, with sides parallel to the field sides). Find the minimum number of extensions needed to reach Arkady's goal.</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>h</i>, <i>w</i>, <i>n</i> ≤ 100 000</span>)&nbsp;— the sizes of the rectangle needed to be placed, the initial sizes of the field and the number of available extensions.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals the integer a side multiplies by when the <span class="tex-span"><i>i</i></span>-th extension is applied.</p></div><div class="output-specification"><p>Print the minimum number of extensions needed to reach Arkady's goal. If it is not possible to place the rectangle on the field with all extensions, print <span class="tex-font-style-tt">-1</span>. If the rectangle can be placed on the initial field, print <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>h</i>, <i>w</i>, <i>n</i> ≤ 100 000</span>)&nbsp;— the sizes of the rectangle needed to be placed, the initial sizes of the field and the number of available extensions.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals the integer a side multiplies by when the <span class="tex-span"><i>i</i></span>-th extension is applied.</p>

## Output

<p>Print the minimum number of extensions needed to reach Arkady's goal. If it is not possible to place the rectangle on the field with all extensions, print <span class="tex-font-style-tt">-1</span>. If the rectangle can be placed on the initial field, print <span class="tex-font-style-tt">0</span>.</p>





```input1
3 3 2 4 4
2 5 4 10

```




```input2
3 3 3 3 5
2 3 5 4 2

```




```input3
5 5 1 2 3
2 2 3

```




```input4
3 4 1 1 3
2 3 2

```




```output1
1

```




```output2
0

```




```output3
-1

```




```output4
3

```



## Note

<p>In the first example it is enough to use any of the extensions available. For example, we can enlarge <span class="tex-span"><i>h</i></span> in <span class="tex-span">5</span> times using the second extension. Then <span class="tex-span"><i>h</i></span> becomes equal <span class="tex-span">10</span> and it is now possible to place the rectangle on the field.</p>
