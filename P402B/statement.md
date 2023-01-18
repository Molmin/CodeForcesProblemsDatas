## Description

<div><p>The Queen of England has <span class="tex-span"><i>n</i></span> trees growing in a row in her garden. At that, the <span class="tex-span"><i>i</i></span>-th <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> tree from the left has height <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> meters. Today the Queen decided to update the scenery of her garden. She wants the trees' heights to meet the condition: for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub> - <i>a</i><sub class="lower-index"><i>i</i></sub> = <i>k</i></span>, where <span class="tex-span"><i>k</i></span> is the number the Queen chose.</p><p>Unfortunately, the royal gardener is not a machine and he cannot fulfill the desire of the Queen instantly! In one minute, the gardener can either decrease the height of a tree to any positive integer height or increase the height of a tree to any positive integer height. How should the royal gardener act to fulfill a whim of Her Majesty in the minimum number of minutes?</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the heights of the trees in the row. </p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>p</i></span> — the minimum number of minutes the gardener needs. In the next <span class="tex-span"><i>p</i></span> lines print the description of his actions. </p><p>If the gardener needs to increase the height of the <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) tree from the left by <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> ≥ 1)</span> meters, then print in the corresponding line "<span class="tex-font-style-tt">+&nbsp;j&nbsp;x</span>". If the gardener needs to decrease the height of the <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) tree from the left by <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> ≥ 1)</span> meters, print on the corresponding line "<span class="tex-font-style-tt">-&nbsp;j&nbsp;x</span>".</p><p>If there are multiple ways to make a row of trees beautiful in the minimum number of actions, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — the heights of the trees in the row. </p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>p</i></span> — the minimum number of minutes the gardener needs. In the next <span class="tex-span"><i>p</i></span> lines print the description of his actions. </p><p>If the gardener needs to increase the height of the <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) tree from the left by <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> ≥ 1)</span> meters, then print in the corresponding line "<span class="tex-font-style-tt">+&nbsp;j&nbsp;x</span>". If the gardener needs to decrease the height of the <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>n</i></span>) tree from the left by <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> ≥ 1)</span> meters, print on the corresponding line "<span class="tex-font-style-tt">-&nbsp;j&nbsp;x</span>".</p><p>If there are multiple ways to make a row of trees beautiful in the minimum number of actions, you are allowed to print any of them.</p>





```input1
4 1
1 2 1 5

```




```input2
4 1
1 2 3 4

```




```output1
2
+ 3 2
- 4 1

```




```output2
0

```


