## Description

<div><p>Assume that <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub>(<i>n</i>)</span> equals the sum of digits of number <span class="tex-span"><i>n</i></span> in the <span class="tex-span"><i>k</i></span>-based notation. For example, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub>(5) = <i>s</i><sub class="lower-index">2</sub>(101<sub class="lower-index">2</sub>) = 1 + 0 + 1 = 2</span>, <span class="tex-span"><i>s</i><sub class="lower-index">3</sub>(14) = <i>s</i><sub class="lower-index">3</sub>(112<sub class="lower-index">3</sub>) = 1 + 1 + 2 = 4</span>.</p><p>The sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> is defined as <img align="middle" class="tex-formula" src="file://YU6s7DTv.png" style="max-width: 100.0%;max-height: 100.0%;">. Your task is to calculate the number of distinct <span class="tex-font-style-underline">subsequences</span> of sequence <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span>. Calculate the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> is called to be a <span class="tex-font-style-underline">subsequence</span> of sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>l</i></sub></span>, if there is a sequence of indices <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub> ≤ <i>l</i></span>, such that <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> = <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub></span>. In particular, an empty sequence (i.e. the sequence consisting of zero elements) is a subsequence of any sequence.</p></div><div class="input-specification"><p>The first line contains two space-separated numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 30</span>).</p></div><div class="output-specification"><p>In a single line print the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two space-separated numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span">2 ≤ <i>k</i> ≤ 30</span>).</p>

## Output

<p>In a single line print the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4 2

```




```input2
7 7

```




```output1
11

```




```output2
128

```



## Note

<p>In the first sample the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> looks as follows: <span class="tex-span">(0, 1, 1, 0)</span>. All the possible subsequences are: </p><center class="tex-equation"><span class="tex-span">(), (0), (0, 0), (0, 1), (0, 1, 0), (0, 1, 1), (0, 1, 1, 0), (1), (1, 0), (1, 1), (1, 1, 0).</span></center><p>In the second sample the sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> looks as follows: <span class="tex-span">(0, 1, 2, 3, 4, 5, 6)</span>. The subsequences of this sequence are exactly all increasing sequences formed from numbers from 0 to 6. It is easy to see that there are <span class="tex-span">2<sup class="upper-index">7</sup> = 128</span> such sequences.</p>
