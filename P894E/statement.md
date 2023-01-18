## Description

<div><p>Ralph is going to collect mushrooms in the Mushroom Forest. </p><p>There are <span class="tex-span"><i>m</i></span> directed paths connecting <span class="tex-span"><i>n</i></span> trees in the Mushroom Forest. On each path grow some mushrooms. When Ralph passes a path, he collects all the mushrooms on the path. The Mushroom Forest has a magical fertile ground where mushrooms grow at a fantastic speed. New mushrooms regrow as soon as Ralph finishes mushroom collection on a path. More specifically, after Ralph passes a path the <span class="tex-span"><i>i</i></span>-th time, there regrow <span class="tex-span"><i>i</i></span> mushrooms less than there was before this pass. That is, if there is initially <span class="tex-span"><i>x</i></span> mushrooms on a path, then Ralph will collect <span class="tex-span"><i>x</i></span> mushrooms for the first time, <span class="tex-span"><i>x</i> - 1</span> mushrooms the second time, <span class="tex-span"><i>x</i> - 1 - 2</span> mushrooms the third time, and so on. However, the number of mushrooms can never be less than <span class="tex-span">0</span>.</p><p>For example, let there be <span class="tex-span">9</span> mushrooms on a path initially. The number of mushrooms that can be collected from the path is <span class="tex-span">9</span>, <span class="tex-span">8</span>, <span class="tex-span">6</span> and <span class="tex-span">3</span> when Ralph passes by from first to fourth time. From the fifth time and later Ralph can't collect any mushrooms from the path (but still can pass it).</p><p>Ralph decided to start from the tree <span class="tex-span"><i>s</i></span>. How many mushrooms can he collect using only described paths?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>), representing the number of trees and the number of directed paths in the Mushroom Forest, respectively.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i> ≤ 10<sup class="upper-index">8</sup></span>), denoting a path that leads from tree <span class="tex-span"><i>x</i></span> to tree <span class="tex-span"><i>y</i></span> with <span class="tex-span"><i>w</i></span> mushrooms initially. There can be paths that lead from a tree to itself, and multiple paths between the same pair of trees.</p><p>The last line contains a single integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the starting position of Ralph. </p></div><div class="output-specification"><p>Print an integer denoting the maximum number of the mushrooms Ralph can collect during his route. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>), representing the number of trees and the number of directed paths in the Mushroom Forest, respectively.</p><p>Each of the following <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>w</i> ≤ 10<sup class="upper-index">8</sup></span>), denoting a path that leads from tree <span class="tex-span"><i>x</i></span> to tree <span class="tex-span"><i>y</i></span> with <span class="tex-span"><i>w</i></span> mushrooms initially. There can be paths that lead from a tree to itself, and multiple paths between the same pair of trees.</p><p>The last line contains a single integer <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the starting position of Ralph. </p>

## Output

<p>Print an integer denoting the maximum number of the mushrooms Ralph can collect during his route. </p>





```input1
2 2
1 2 4
2 1 4
1

```




```input2
3 3
1 2 4
2 3 3
1 3 8
1

```




```output1
16
```




```output2
8
```



## Note

<p>In the first sample Ralph can pass three times on the circle and collect <span class="tex-span">4 + 4 + 3 + 3 + 1 + 1 = 16</span> mushrooms. After that there will be no mushrooms for Ralph to collect.</p><p>In the second sample, Ralph can go to tree <span class="tex-span">3</span> and collect <span class="tex-span">8</span> mushrooms on the path from tree <span class="tex-span">1</span> to tree <span class="tex-span">3</span>.</p>
