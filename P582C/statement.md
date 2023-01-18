## Description

<div><p>You are given an infinite periodic array <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub>, ...</span> with the period of length <span class="tex-span"><i>n</i></span>. Formally, <img align="middle" class="tex-formula" src="file://xzslPthQ.png" style="max-width: 100.0%;max-height: 100.0%;">. A periodic subarray <span class="tex-span">(<i>l</i>, <i>s</i>)</span> (<span class="tex-span">0 ≤ <i>l</i> &lt; <i>n</i></span>, <span class="tex-span">1 ≤ <i>s</i> &lt; <i>n</i></span>) of array <span class="tex-span"><i>a</i></span> is an infinite periodic array with a period of length <span class="tex-span"><i>s</i></span> that is a subsegment of array <span class="tex-span"><i>a</i></span>, starting with position <span class="tex-span"><i>l</i></span>.</p><p>A periodic subarray <span class="tex-span">(<i>l</i>, <i>s</i>)</span> is <span class="tex-font-style-it">superior</span>, if when attaching it to the array <span class="tex-span"><i>a</i></span>, starting from index <span class="tex-span"><i>l</i></span>, any element of the subarray is larger than or equal to the corresponding element of array <span class="tex-span"><i>a</i></span>. An example of attaching is given on the figure (top — infinite array <span class="tex-span"><i>a</i></span>, bottom — its periodic subarray <span class="tex-span">(<i>l</i>, <i>s</i>)</span>):</p><center> <img class="tex-graphics" src="file://aHHdJs0R.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Find the number of distinct pairs <span class="tex-span">(<i>l</i>, <i>s</i>)</span>, corresponding to the superior periodic arrays.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), separated by a space.</p></div><div class="output-specification"><p>Print a single integer — the sought number of pairs.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), separated by a space.</p>

## Output

<p>Print a single integer — the sought number of pairs.</p>





```input1
4
7 1 2 3

```




```input2
2
2 1

```




```input3
3
1 1 1

```




```output1
2

```




```output2
1

```




```output3
6

```



## Note

<p>In the first sample the superior subarrays are (0, 1) and (3, 2).</p><p>Subarray (0, 1) is superior, as <span class="tex-span"><i>a</i><sub class="lower-index">0</sub> ≥ <i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">0</sub> ≥ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">0</sub> ≥ <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">0</sub> ≥ <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">0</sub> ≥ <i>a</i><sub class="lower-index">0</sub>, ...</span></p><p>Subarray (3, 2) is superior <span class="tex-span"><i>a</i><sub class="lower-index">3</sub> ≥ <i>a</i><sub class="lower-index">3</sub>, <i>a</i><sub class="lower-index">0</sub> ≥ <i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">3</sub> ≥ <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">0</sub> ≥ <i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub> ≥ <i>a</i><sub class="lower-index">3</sub>, ...</span></p><p>In the third sample any pair of <span class="tex-span">(<i>l</i>, <i>s</i>)</span> corresponds to a superior subarray as all the elements of an array are distinct.</p>
