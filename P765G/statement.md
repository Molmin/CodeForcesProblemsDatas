## Description

<div><p><span class="tex-font-style-it">If you have gone that far, you'll probably skip unnecessary legends anyway...</span></p><p>You are given a binary string <img align="middle" class="tex-formula" src="file://PjZONrQF.png" style="max-width: 100.0%;max-height: 100.0%;"> and an integer <img align="middle" class="tex-formula" src="file://3LuQ4Re9.png" style="max-width: 100.0%;max-height: 100.0%;">. Find the number of integers <span class="tex-span"><i>k</i></span>, <span class="tex-span">0 ≤ <i>k</i> &lt; <i>N</i></span>, such that for all <span class="tex-span"><i>i</i> = 0</span>, <span class="tex-span">1</span>, ..., <span class="tex-span"><i>m</i> - 1</span> </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://hYv6MUR3.png" style="max-width: 100.0%;max-height: 100.0%;"></center> Print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</div><div class="input-specification"><p>In the first line of input there is a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span">0</span>'s and <span class="tex-span">1</span>'s (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 40</span>).</p><p>In the next line of input there is an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">α<sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, α<sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is prime). All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>A single integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>In the first line of input there is a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span">0</span>'s and <span class="tex-span">1</span>'s (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 40</span>).</p><p>In the next line of input there is an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">α<sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, α<sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is prime). All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>A single integer&nbsp;— the answer to the problem.</p>





```input1
1
2
2 1
3 1

```




```input2
01
2
3 2
5 1

```




```input3
1011
1
3 1000000000

```




```output1
2

```




```output2
15

```




```output3
411979884

```


