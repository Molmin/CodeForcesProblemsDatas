## Description

<div><p>Alexandra has a paper strip with <span class="tex-span"><i>n</i></span> numbers on it. Let's call them <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from left to right.</p><p>Now Alexandra wants to split it into some pieces (possibly <span class="tex-span">1</span>). For each piece of strip, it must satisfy:</p><ul><li> Each piece should contain at least <span class="tex-span"><i>l</i></span> numbers.</li><li> The difference between the maximal and the minimal number on the piece should be at most <span class="tex-span"><i>s</i></span>.</li></ul><p>Please help Alexandra to find the minimal number of pieces meeting the condition above.</p></div><div class="input-specification"><p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>s</i>, <i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>l</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> separated by spaces (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output the minimal number of strip pieces.</p><p>If there are no ways to split the strip, output -1.</p></div>

## Input

<p>The first line contains three space-separated integers <span class="tex-span"><i>n</i>, <i>s</i>, <i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>l</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> separated by spaces (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output the minimal number of strip pieces.</p><p>If there are no ways to split the strip, output -1.</p>





```input1
7 2 2
1 3 1 2 4 1 2

```




```input2
7 2 2
1 100 1 100 1 100 1

```




```output1
3

```




```output2
-1

```



## Note

<p>For the first sample, we can split the strip into <span class="tex-span">3</span> pieces: <span class="tex-span">[1, 3, 1], [2, 4], [1, 2]</span>.</p><p>For the second sample, we can't let <span class="tex-span">1</span> and <span class="tex-span">100</span> be on the same piece, so no solution exists.</p>
