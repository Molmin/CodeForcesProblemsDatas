## Description

<div><p>After a wonderful evening in the restaurant the time to go home came. Leha as a true gentlemen suggested Noora to give her a lift. Certainly the girl agreed with pleasure. Suddenly one problem appeared: Leha cannot find his car on a huge parking near the restaurant. So he decided to turn to the watchman for help.</p><p>Formally the parking can be represented as a matrix <span class="tex-span">10<sup class="upper-index">9</sup> × 10<sup class="upper-index">9</sup></span>. There is exactly one car in every cell of the matrix. All cars have their own machine numbers represented as a positive integer. Let's index the columns of the matrix by integers from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span> from left to right and the rows by integers from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span> from top to bottom. By coincidence it turned out, that for every cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> the number of the car, which stands in this cell, is equal to the minimum positive integer, which can't be found in the cells <span class="tex-span">(<i>i</i>, <i>y</i>)</span> and <span class="tex-span">(<i>x</i>, <i>j</i>)</span>, <span class="tex-span">1 ≤ <i>i</i> &lt; <i>x</i>, 1 ≤ <i>j</i> &lt; <i>y</i></span>.</p><center> <img class="tex-graphics" src="file://PnpuvA34.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The upper left fragment <span class="tex-span">5 × 5</span> of the parking</span> </center><p>Leha wants to ask the watchman <span class="tex-span"><i>q</i></span> requests, which can help him to find his car. Every request is represented as five integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>k</i></span>. The watchman have to consider all cells <span class="tex-span">(<i>x</i>, <i>y</i>)</span> of the matrix, such that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i> ≤ <i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i> ≤ <i>y</i><sub class="lower-index">2</sub></span>, and if the number of the car in cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span> does not exceed <span class="tex-span"><i>k</i></span>, increase the answer to the request by the number of the car in cell <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. For each request Leha asks the watchman to tell him the resulting sum. Due to the fact that the sum can turn out to be quite large, hacker asks to calculate it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>However the requests seem to be impracticable for the watchman. Help the watchman to answer all Leha's requests.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">4</sup>)</span>&nbsp;— the number of Leha's requests.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain five integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>&nbsp;— parameters of Leha's requests.</p></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>q</i></span> lines&nbsp;— in the first line print the answer to the first request, in the second&nbsp;— the answer to the second request and so on.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">4</sup>)</span>&nbsp;— the number of Leha's requests.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain five integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>, <i>k</i></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>y</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>&nbsp;— parameters of Leha's requests.</p>

## Output

<p>Print exactly <span class="tex-span"><i>q</i></span> lines&nbsp;— in the first line print the answer to the first request, in the second&nbsp;— the answer to the second request and so on.</p>





```input1
4
1 1 1 1 1
3 2 5 4 5
1 1 5 5 10000
1 4 2 5 2

```




```output1
1
13
93
0

```



## Note

<p>Let's analyze all the requests. In each case the requested submatrix is highlighted in blue.</p><p>In the first request <span class="tex-span">(<i>k</i> = 1)</span> Leha asks only about the upper left parking cell. In this cell the car's number is <span class="tex-span">1</span>. Consequentally the answer is <span class="tex-span">1</span>.</p><p><img class="tex-graphics" src="file://QriFykFq.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second request <span class="tex-span">(<i>k</i> = 5)</span> suitable numbers are <span class="tex-span">4, 1, 2, 3, 2, 1</span>. Consequentally the answer is <span class="tex-span">4 + 1 + 2 + 3 + 2 + 1 = 13</span>.</p><p><img class="tex-graphics" src="file://i40lhx1d.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the third request <span class="tex-span">(<i>k</i> = 10000)</span> Leha asks about the upper left frament <span class="tex-span">5 × 5</span> of the parking. Since <span class="tex-span"><i>k</i></span> is big enough, the answer is equal to <span class="tex-span">93</span>.</p><p><img class="tex-graphics" src="file://uZLDdV77.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the last request <span class="tex-span">(<i>k</i> = 2)</span> none of the cur's numbers are suitable, so the answer is <span class="tex-span">0</span>.</p><p><img class="tex-graphics" src="file://0IpKnH6T.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
