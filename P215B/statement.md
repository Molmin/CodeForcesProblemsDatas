## Description

<div><p>The World Programming Olympics Medal is a metal disk, consisting of two parts: the first part is a ring with outer radius of <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> cm, inner radius of <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> cm, <span class="tex-span">(0 &lt; <i>r</i>2 &lt; <i>r</i>1)</span> made of metal with density <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> g/cm<span class="tex-span"><sup class="upper-index">3</sup></span>. The second part is an inner disk with radius <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> cm, it is made of metal with density <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> g/cm<span class="tex-span"><sup class="upper-index">3</sup></span>. The disk is nested inside the ring.</p><p>The Olympic jury decided that <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> will take one of possible values of <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. It is up to jury to decide which particular value <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span> will take. Similarly, the Olympic jury decided that <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> will take one of possible value of <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span>, and <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> will take a value from list <span class="tex-span"><i>z</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">2</sub>, ..., <i>z</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>According to most ancient traditions the ratio between the outer ring mass <span class="tex-span"><i>m</i><sub class="lower-index"><i>out</i></sub></span> and the inner disk mass <span class="tex-span"><i>m</i><sub class="lower-index"><i>in</i></sub></span> must equal <img align="middle" class="tex-formula" src="file://Zb8g7d2T.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>A</i>, <i>B</i></span> are constants taken from ancient books. Now, to start making medals, the jury needs to take values for <span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub></span> and calculate the suitable value of <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>.</p><p>The jury wants to choose the value that would maximize radius <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>. Help the jury find the sought value of <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>. Value <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> doesn't have to be an integer.</p><p>Medal has a uniform thickness throughout the area, the thickness of the inner disk is the same as the thickness of the outer ring.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> and a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. The second input line contains an integer <span class="tex-span"><i>m</i></span> and a sequence of integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span>. The third input line contains an integer <span class="tex-span"><i>k</i></span> and a sequence of integers <span class="tex-span"><i>z</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">2</sub>, ..., <i>z</i><sub class="lower-index"><i>k</i></sub></span>. The last line contains two integers <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>.</p><p>All numbers given in the input are positive and do not exceed 5000. Each of the three sequences contains distinct numbers. The numbers in the lines are separated by spaces.</p></div><div class="output-specification"><p>Print a single real number — the sought value <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> with absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. It is guaranteed that the solution that meets the problem requirements exists.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> and a sequence of integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. The second input line contains an integer <span class="tex-span"><i>m</i></span> and a sequence of integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span>. The third input line contains an integer <span class="tex-span"><i>k</i></span> and a sequence of integers <span class="tex-span"><i>z</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">2</sub>, ..., <i>z</i><sub class="lower-index"><i>k</i></sub></span>. The last line contains two integers <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>.</p><p>All numbers given in the input are positive and do not exceed 5000. Each of the three sequences contains distinct numbers. The numbers in the lines are separated by spaces.</p>

## Output

<p>Print a single real number — the sought value <span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span> with absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. It is guaranteed that the solution that meets the problem requirements exists.</p>





```input1
3 1 2 3
1 2
3 3 2 1
1 2

```




```input2
4 2 3 6 4
2 1 2
3 10 6 8
2 1

```




```output1
2.683281573000

```




```output2
2.267786838055

```



## Note

<p>In the first sample the jury should choose the following values: <span class="tex-span"><i>r</i><sub class="lower-index">1</sub> = 3</span>, <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> = 2</span>, <span class="tex-span"><i>p</i><sub class="lower-index">2</sub> = 1</span>.</p>
