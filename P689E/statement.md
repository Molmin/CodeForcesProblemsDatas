## Description

<div><p>Mike wants to prepare for IMO but he doesn't know geometry, so his teacher gave him an interesting geometry problem. Let's define <span class="tex-span"><i>f</i>([<i>l</i>, <i>r</i>]) = <i>r</i> - <i>l</i> + 1</span> to be the number of integer points in the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> with <span class="tex-span"><i>l</i> ≤ <i>r</i></span> (say that <img align="middle" class="tex-formula" src="file://arJ62Nhd.png" style="max-width: 100.0%;max-height: 100.0%;">). You are given two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>n</i></span> closed intervals <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> on <span class="tex-span"><i>OX</i></span> axis and you have to find:</p><center> <img align="middle" class="tex-formula" src="file://PrR0CL9D.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In other words, you should find the sum of the number of integer points in the intersection of any <span class="tex-span"><i>k</i></span> of the segments. </p><p>As the answer may be very large, output it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p><p>Mike can't solve this problem so he needs your help. You will help him, won't you? </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of segments and the number of segments in intersection groups respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, describing <span class="tex-span"><i>i</i></span>-th segment bounds.</p></div><div class="output-specification"><p>Print one integer number&nbsp;— the answer to Mike's problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>) in the only line.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of segments and the number of segments in intersection groups respectively.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">9</sup> ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, describing <span class="tex-span"><i>i</i></span>-th segment bounds.</p>

## Output

<p>Print one integer number&nbsp;— the answer to Mike's problem modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>) in the only line.</p>





```input1
3 2
1 2
1 3
2 3

```




```input2
3 3
1 3
1 3
1 3

```




```input3
3 1
1 2
2 3
3 4

```




```output1
5

```




```output2
3

```




```output3
6

```



## Note

<p>In the first example: </p><p><img align="middle" class="tex-formula" src="file://sBYcR0aO.png" style="max-width: 100.0%;max-height: 100.0%;">;</p><p><img align="middle" class="tex-formula" src="file://an3FVWmh.png" style="max-width: 100.0%;max-height: 100.0%;">;</p><p><img align="middle" class="tex-formula" src="file://wiN5HrhP.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>So the answer is <span class="tex-span">2 + 1 + 2 = 5</span>.</p>
