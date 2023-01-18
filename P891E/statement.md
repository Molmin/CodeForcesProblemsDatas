## Description

<div><p><span class="tex-font-style-it">A false witness that speaketh lies!</span></p><p>You are given a sequence containing <span class="tex-span"><i>n</i></span> integers. There is a variable <span class="tex-span"><i>res</i></span> that is equal to <span class="tex-span">0</span> initially. The following process repeats <span class="tex-span"><i>k</i></span> times.</p><p>Choose an index from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> uniformly at random. Name it <span class="tex-span"><i>x</i></span>. Add to <span class="tex-span"><i>res</i></span> the multiply of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>'s such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, but <span class="tex-span"><i>i</i> ≠ <i>x</i></span>. Then, subtract <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub></span> by <span class="tex-span">1</span>.</p><p>You have to find expected value of <span class="tex-span"><i>res</i></span> at the end of the process. It can be proved that the expected value of <span class="tex-span"><i>res</i></span> can be represented as an irreducible fraction <img align="middle" class="tex-formula" src="file://RzcfmomS.png" style="max-width: 100.0%;max-height: 100.0%;">. You have to find <img align="middle" class="tex-formula" src="file://5P27mwUo.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements and parameter <span class="tex-span"><i>k</i></span> that is specified in the statement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the value <img align="middle" class="tex-formula" src="file://z6ahyGY8.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of elements and parameter <span class="tex-span"><i>k</i></span> that is specified in the statement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Output a single integer&nbsp;— the value <img align="middle" class="tex-formula" src="file://z6ahyGY8.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 1
5 5

```




```input2
1 10
80

```




```input3
2 2
0 0

```




```input4
9 4
0 11 12 9 20 7 8 18 2

```




```output1
5
```




```output2
10
```




```output3
500000003
```




```output4
169316356
```


