## Description

<div><p>Jzzhu has invented a kind of sequences, they meet the following property:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://DKLTWaKZ.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>You are given <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, please calculate <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i></sub></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(|<i>x</i>|, |<i>y</i>| ≤ 10<sup class="upper-index">9</sup>)</span>. The second line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Output a single integer representing <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i></sub></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(|<i>x</i>|, |<i>y</i>| ≤ 10<sup class="upper-index">9</sup>)</span>. The second line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Output a single integer representing <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i></sub></span> modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2 3
3

```




```input2
0 -1
2

```




```output1
1

```




```output2
1000000006

```



## Note

<p>In the first sample, <span class="tex-span"><i>f</i><sub class="lower-index">2</sub> = <i>f</i><sub class="lower-index">1</sub> + <i>f</i><sub class="lower-index">3</sub></span>, <span class="tex-span">3 = 2 + <i>f</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index">3</sub> = 1</span>.</p><p>In the second sample, <span class="tex-span"><i>f</i><sub class="lower-index">2</sub> =  - 1</span>; <span class="tex-span"> - 1</span> modulo <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span> equals <span class="tex-span">(10<sup class="upper-index">9</sup> + 6)</span>.</p>
