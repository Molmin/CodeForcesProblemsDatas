## Description

<div><p>You are given three integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>a</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>b</i></sub></span>.</p><p>You will construct a sequence with the following algorithm: Initially, start with the empty sequence. Each second, you do the following. With probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>a</i></sub> / (<i>p</i><sub class="lower-index"><i>a</i></sub> + <i>p</i><sub class="lower-index"><i>b</i></sub>)</span>, add '<span class="tex-font-style-tt">a</span>' to the end of the sequence. Otherwise (with probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>b</i></sub> / (<i>p</i><sub class="lower-index"><i>a</i></sub> + <i>p</i><sub class="lower-index"><i>b</i></sub>)</span>), add '<span class="tex-font-style-tt">b</span>' to the end of the sequence.</p><p>You stop once there are at least <span class="tex-span"><i>k</i></span> subsequences that form '<span class="tex-font-style-tt">ab</span>'. Determine the expected number of times '<span class="tex-font-style-tt">ab</span>' is a subsequence in the resulting sequence. It can be shown that this can be represented by <span class="tex-span"><i>P</i> / <i>Q</i></span>, where <span class="tex-span"><i>P</i></span> and <span class="tex-span"><i>Q</i></span> are coprime integers, and <img align="middle" class="tex-formula" src="file://wzA98jHg.png" style="max-width: 100.0%;max-height: 100.0%;">. Print the value of <img align="middle" class="tex-formula" src="file://jFcDmZ6Z.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line will contain three integers integer <span class="tex-span"><i>k</i>, <i>p</i><sub class="lower-index"><i>a</i></sub>, <i>p</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>a</i></sub>, <i>p</i><sub class="lower-index"><i>b</i></sub> ≤ 1 000 000</span>).</p></div><div class="output-specification"><p>Print a single integer, the answer to the problem.</p></div>

## Input

<p>The first line will contain three integers integer <span class="tex-span"><i>k</i>, <i>p</i><sub class="lower-index"><i>a</i></sub>, <i>p</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 1 000</span>, <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>a</i></sub>, <i>p</i><sub class="lower-index"><i>b</i></sub> ≤ 1 000 000</span>).</p>

## Output

<p>Print a single integer, the answer to the problem.</p>





```input1
1 1 1

```




```input2
3 1 4

```




```output1
2

```




```output2
370000006

```



## Note

<p>The first sample, we will keep appending to our sequence until we get the subsequence '<span class="tex-font-style-tt">ab</span>' at least once. For instance, we get the sequence '<span class="tex-font-style-tt">ab</span>' with probability 1/4, '<span class="tex-font-style-tt">bbab</span>' with probability 1/16, and '<span class="tex-font-style-tt">aab</span>' with probability 1/8. Note, it's impossible for us to end with a sequence like '<span class="tex-font-style-tt">aabab</span>', since we would have stopped our algorithm once we had the prefix '<span class="tex-font-style-tt">aab</span>'. </p><p>The expected amount of times that '<span class="tex-font-style-tt">ab</span>' will occur across all valid sequences is 2. </p><p>For the second sample, the answer is equal to <img align="middle" class="tex-formula" src="file://UvzvQw6E.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
