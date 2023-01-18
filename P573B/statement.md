## Description

<div><p>Limak is a little bear who loves to play. Today he is playing by destroying block towers. He built <span class="tex-span"><i>n</i></span> towers in a row. The <span class="tex-span"><i>i</i></span>-th tower is made of <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> identical blocks. For clarification see picture for the first sample.</p><p>Limak will repeat the following operation till everything is destroyed.</p><p>Block is called internal if it has all four neighbors, i.e. it has each side (top, left, down and right) adjacent to other block or to the floor. Otherwise, block is boundary. In one operation Limak destroys all boundary blocks. His paws are very fast and he destroys all those blocks at the same time.</p><p>Limak is ready to start. You task is to count how many operations will it take him to destroy all towers.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — sizes of towers.</p></div><div class="output-specification"><p>Print the number of operations needed to destroy all towers.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — sizes of towers.</p>

## Output

<p>Print the number of operations needed to destroy all towers.</p>





```input1
6
2 1 4 6 2 2

```




```input2
7
3 3 3 1 3 3 3

```




```output1
3

```




```output2
2

```



## Note

<p>The picture below shows all three operations for the first sample test. Each time boundary blocks are marked with red color. </p><center> <img class="tex-graphics" src="file://jxL5lnkB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> After first operation there are four blocks left and only one remains after second operation. This last block is destroyed in third operation.
