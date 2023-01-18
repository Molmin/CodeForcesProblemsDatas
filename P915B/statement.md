## Description

<div><p>Luba is surfing the Internet. She currently has <span class="tex-span"><i>n</i></span> opened tabs in her browser, indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. The mouse cursor is currently located at the <span class="tex-span"><i>pos</i></span>-th tab. Luba needs to use the tabs with indices from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (inclusive) for her studies, and she wants to close all the tabs that don't belong to this segment as fast as possible.</p><p>Each second Luba can either try moving the cursor to the left or to the right (if the cursor is currently at the tab <span class="tex-span"><i>i</i></span>, then she can move it to the tab <span class="tex-span"><i>max</i>(<i>i</i> - 1, <i>a</i>)</span> or to the tab <span class="tex-span"><i>min</i>(<i>i</i> + 1, <i>b</i>)</span>) or try closing all the tabs to the left or to the right of the cursor (if the cursor is currently at the tab <span class="tex-span"><i>i</i></span>, she can close all the tabs with indices from segment <span class="tex-span">[<i>a</i>, <i>i</i> - 1]</span> or from segment <span class="tex-span">[<i>i</i> + 1, <i>b</i>]</span>). In the aforementioned expressions <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> denote the minimum and maximum index of an unclosed tab, respectively. For example, if there were <span class="tex-span">7</span> tabs initially and tabs <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">7</span> are closed, then <span class="tex-span"><i>a</i> = 3</span>, <span class="tex-span"><i>b</i> = 6</span>.</p><p>What is the minimum number of seconds Luba has to spend in order to leave <span class="tex-font-style-bf">only the tabs with initial indices from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusive</span> opened?</p></div><div class="input-specification"><p>The only line of input contains four integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>pos</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>pos</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) — the number of the tabs, the cursor position and the segment which Luba needs to leave opened.</p></div><div class="output-specification"><p>Print one integer equal to the minimum number of seconds required to close all the tabs outside the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>.</p></div>

## Input

<p>The only line of input contains four integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>pos</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>pos</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>) — the number of the tabs, the cursor position and the segment which Luba needs to leave opened.</p>

## Output

<p>Print one integer equal to the minimum number of seconds required to close all the tabs outside the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>.</p>





```input1
6 3 2 4

```




```input2
6 3 1 3

```




```input3
5 2 1 5

```




```output1
5

```




```output2
1

```




```output3
0

```



## Note

<p>In the first test Luba can do the following operations: shift the mouse cursor to the tab <span class="tex-span">2</span>, close all the tabs to the left of it, shift the mouse cursor to the tab <span class="tex-span">3</span>, then to the tab <span class="tex-span">4</span>, and then close all the tabs to the right of it.</p><p>In the second test she only needs to close all the tabs to the right of the current position of the cursor.</p><p>In the third test Luba doesn't need to do anything.</p>
