## Description

<div><p>You have <span class="tex-span"><i>n</i></span> distinct points on a plane, none of them lie on <span class="tex-span"><i>OY</i></span> axis. Check that there is a point after removal of which the remaining points are located on one side of the <span class="tex-span"><i>OY</i></span> axis.</p></div><div class="input-specification"><p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following <span class="tex-span"><i>n</i></span> lines contain coordinates of the points. The <span class="tex-span"><i>i</i></span>-th of these lines contains two single integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>). No two points coincide.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if there is such a point, "<span class="tex-font-style-tt">No</span>" — otherwise.</p><p>You can print every letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following <span class="tex-span"><i>n</i></span> lines contain coordinates of the points. The <span class="tex-span"><i>i</i></span>-th of these lines contains two single integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i><sub class="lower-index"><i>i</i></sub>|, |<i>y</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>). No two points coincide.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if there is such a point, "<span class="tex-font-style-tt">No</span>" — otherwise.</p><p>You can print every letter in any case (upper or lower).</p>





```input1
3
1 1
-1 -1
2 -1

```




```input2
4
1 1
2 2
-1 1
-2 2

```




```input3
3
1 2
2 1
4 60

```




```output1
Yes
```




```output2
No
```




```output3
Yes
```



## Note

<p>In the first example the second point can be removed.</p><p>In the second example there is no suitable for the condition point.</p><p>In the third example any point can be removed.</p>
