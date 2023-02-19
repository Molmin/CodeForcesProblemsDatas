## Description

<div><p>Mahmoud has <span class="tex-span"><i>n</i></span> line segments, the <span class="tex-span"><i>i</i></span>-th of them has length <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Ehab challenged him to use <span class="tex-font-style-bf">exactly <span class="tex-span">3</span></span> line segments to form a non-degenerate triangle. Mahmoud doesn't accept challenges unless he is sure he can win, so he asked you to tell him if he should accept the challenge. Given the lengths of the line segments, check if he can choose exactly <span class="tex-span">3</span> of them to form a non-degenerate triangle.</p><p>Mahmoud should use exactly <span class="tex-span">3</span> line segments, he can't concatenate two line segments or change any length. A non-degenerate triangle is a triangle with positive area.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of line segments Mahmoud has.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the lengths of line segments Mahmoud has.</p></div><div class="output-specification"><p>In the only line print "<span class="tex-font-style-tt">YES</span>" if he can choose exactly three line segments and form a non-degenerate triangle with them, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of line segments Mahmoud has.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the lengths of line segments Mahmoud has.</p>

## Output

<p>In the only line print "<span class="tex-font-style-tt">YES</span>" if he can choose exactly three line segments and form a non-degenerate triangle with them, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
5
1 5 3 2 4

```




```input2
3
4 1 2

```




```output1
YES

```




```output2
NO

```



## Note

<p>For the first example, he can use line segments with lengths <span class="tex-span">2</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span> to form a non-degenerate triangle.</p>
