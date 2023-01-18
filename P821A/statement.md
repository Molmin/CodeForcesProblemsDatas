## Description

<div><p>Okabe needs to renovate the <span class="tex-font-style-it">Future Gadget Laboratory</span> after he tried doing some crazy experiments! The lab is represented as an <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>n</i></span> square grid of integers. A <span class="tex-font-style-it">good</span> lab is defined as a lab in which every number not equal to <span class="tex-span">1</span> can be expressed as the sum of a number in the same row and a number in the same column. In other words, for every <span class="tex-span"><i>x</i>, <i>y</i></span> such that <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i>, <i>y</i></sub> ≠ 1</span>, there should exist two indices <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> so that <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i>, <i>y</i></sub> = <i>a</i><sub class="lower-index"><i>x</i>, <i>s</i></sub> + <i>a</i><sub class="lower-index"><i>t</i>, <i>y</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> denotes the integer in <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column.</p><p>Help Okabe determine whether a given lab is <span class="tex-font-style-it">good</span>!</p></div><div class="input-specification"><p>The first line of input contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the size of the lab. </p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> space-separated integers denoting a row of the grid. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th row is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Yes</span>" if the given lab is <span class="tex-font-style-it">good</span> and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in upper or lower case.</p></div>

## Input

<p>The first line of input contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>)&nbsp;— the size of the lab. </p><p>The next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>n</i></span> space-separated integers denoting a row of the grid. The <span class="tex-span"><i>j</i></span>-th integer in the <span class="tex-span"><i>i</i></span>-th row is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print "<span class="tex-font-style-tt">Yes</span>" if the given lab is <span class="tex-font-style-it">good</span> and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in upper or lower case.</p>





```input1
3
1 1 2
2 3 1
6 4 1

```




```input2
3
1 5 2
1 1 1
1 2 3

```




```output1
Yes

```




```output2
No

```



## Note

<p>In the first sample test, the <span class="tex-span">6</span> in the bottom left corner is valid because it is the sum of the <span class="tex-span">2</span> above it and the <span class="tex-span">4</span> on the right. The same holds for every number not equal to <span class="tex-span">1</span> in this table, so the answer is "<span class="tex-font-style-tt">Yes</span>".</p><p>In the second sample test, the <span class="tex-span">5</span> cannot be formed as the sum of an integer in the same row and an integer in the same column. Thus the answer is "<span class="tex-font-style-tt">No</span>".</p>
