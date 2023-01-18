## Description

<div><p>DZY has a sequence <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers.</p><p>We'll call a sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>j</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>j</i> ≤ <i>n</i>)</span> a subsegment of the sequence <span class="tex-span"><i>a</i></span>. The value <span class="tex-span">(<i>j</i> - <i>i</i> + 1)</span> denotes the length of the subsegment.</p><p>Your task is to find the longest subsegment of <span class="tex-span"><i>a</i></span>, such that it is possible to change at most one number (change one number to any integer you want) from the subsegment to make the subsegment strictly increasing.</p><p>You only need to output the length of the subsegment you find.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>In a single line print the answer to the problem — the maximum length of the required subsegment.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>In a single line print the answer to the problem — the maximum length of the required subsegment.</p>





```input1
6
7 2 3 1 5 6

```




```output1
5

```



## Note

<p>You can choose subsegment <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">4</sub>, <i>a</i><sub class="lower-index">5</sub>, <i>a</i><sub class="lower-index">6</sub></span> and change its 3rd element (that is <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span>) to 4.</p>
