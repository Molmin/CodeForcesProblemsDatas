## Description

<div><p>Simon has a prime number <span class="tex-span"><i>x</i></span> and an array of non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>.</p><p>Simon loves fractions very much. Today he wrote out number <img align="middle" class="tex-formula" src="file://cY0wDMXV.png" style="max-width: 100.0%;max-height: 100.0%;"> on a piece of paper. After Simon led all fractions to a common denominator and summed them up, he got a fraction: <img align="middle" class="tex-formula" src="file://NRBJlp3G.png" style="max-width: 100.0%;max-height: 100.0%;">, where number <span class="tex-span"><i>t</i></span> equals <span class="tex-span"><i>x</i><sup class="upper-index"><i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub></sup></span>. Now Simon wants to reduce the resulting fraction. </p><p>Help him, find the greatest common divisor of numbers <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. As GCD can be rather large, print it as a remainder after dividing it by number <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) — the size of the array and the prime number.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p></div><div class="output-specification"><p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>) — the size of the array and the prime number.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </p>

## Output

<p>Print a single number — the answer to the problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
2 2
2 2

```




```input2
3 3
1 2 3

```




```input3
2 2
29 29

```




```input4
4 5
0 0 0 0

```




```output1
8

```




```output2
27

```




```output3
73741817

```




```output4
1

```



## Note

<p>In the first sample <img align="middle" class="tex-formula" src="file://40ycXnns.png" style="max-width: 100.0%;max-height: 100.0%;">. Thus, the answer to the problem is <span class="tex-span">8</span>.</p><p>In the second sample, <img align="middle" class="tex-formula" src="file://BLZmPQsM.png" style="max-width: 100.0%;max-height: 100.0%;">. The answer to the problem is <span class="tex-span">27</span>, as <span class="tex-span">351 = 13·27</span>, <span class="tex-span">729 = 27·27</span>.</p><p>In the third sample the answer to the problem is <span class="tex-span">1073741824&nbsp;<i>mod</i>&nbsp;1000000007 = 73741817</span>.</p><p>In the fourth sample <img align="middle" class="tex-formula" src="file://tc2nCbSH.png" style="max-width: 100.0%;max-height: 100.0%;">. Thus, the answer to the problem is <span class="tex-span">1</span>.</p>
