## Description

<div><p>Let's denote as <img align="middle" class="tex-formula" src="file://PHRs99bw.png" style="max-width: 100.0%;max-height: 100.0%;"> the number of bits set ('1' bits) in the binary representation of the non-negative integer <span class="tex-span"><i>x</i></span>.</p><p>You are given multiple queries consisting of pairs of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. For each query, find the <span class="tex-span"><i>x</i></span>, such that <span class="tex-span"><i>l</i> ≤ <i>x</i> ≤ <i>r</i></span>, and <img align="middle" class="tex-formula" src="file://hdIebsKn.png" style="max-width: 100.0%;max-height: 100.0%;"> is maximum possible. If there are multiple such numbers find the smallest of them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of queries (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>).</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the arguments for the corresponding query (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>For each query print the answer in a separate line.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of queries (<span class="tex-span">1 ≤ <i>n</i> ≤ 10000</span>).</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the arguments for the corresponding query (<span class="tex-span">0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>For each query print the answer in a separate line.</p>





```input1
3
1 2
2 4
1 10

```




```output1
1
3
7

```



## Note

<p>The binary representations of numbers from 1 to 10 are listed below:</p><p><span class="tex-span">1<sub class="lower-index">10</sub> = 1<sub class="lower-index">2</sub></span></p><p><span class="tex-span">2<sub class="lower-index">10</sub> = 10<sub class="lower-index">2</sub></span></p><p><span class="tex-span">3<sub class="lower-index">10</sub> = 11<sub class="lower-index">2</sub></span></p><p><span class="tex-span">4<sub class="lower-index">10</sub> = 100<sub class="lower-index">2</sub></span></p><p><span class="tex-span">5<sub class="lower-index">10</sub> = 101<sub class="lower-index">2</sub></span></p><p><span class="tex-span">6<sub class="lower-index">10</sub> = 110<sub class="lower-index">2</sub></span></p><p><span class="tex-span">7<sub class="lower-index">10</sub> = 111<sub class="lower-index">2</sub></span></p><p><span class="tex-span">8<sub class="lower-index">10</sub> = 1000<sub class="lower-index">2</sub></span></p><p><span class="tex-span">9<sub class="lower-index">10</sub> = 1001<sub class="lower-index">2</sub></span></p><p><span class="tex-span">10<sub class="lower-index">10</sub> = 1010<sub class="lower-index">2</sub></span></p>
