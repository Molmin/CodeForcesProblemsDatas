## Description

<div><p>The sequence of integer pairs <span class="tex-span">(<i>a</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">1</sub>), (<i>a</i><sub class="lower-index">2</sub>, <i>b</i><sub class="lower-index">2</sub>), ..., (<i>a</i><sub class="lower-index"><i>k</i></sub>, <i>b</i><sub class="lower-index"><i>k</i></sub>)</span> is <span class="tex-font-style-it">beautiful</span>, if the following statements are fulfilled: </p><ul> <li> <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index">1</sub> ≤ <i>b</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> ≤ <i>b</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ <i>b</i><sub class="lower-index"><i>k</i></sub> ≤ <i>n</i></span>, where <span class="tex-span"><i>n</i></span> is a given positive integer; </li><li> all numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub> - <i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub> - <i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>k</i></sub> - <i>a</i><sub class="lower-index"><i>k</i></sub></span> are distinct. </li></ul><p>For the given number <span class="tex-span"><i>n</i></span> find the number of beautiful sequences of length <span class="tex-span"><i>k</i></span>. As the answer can be rather large, print the remainder after dividing it by <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤  2·10<sup class="upper-index">5</sup></span>) — the number of the test data.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>For each test from the input print the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. Print the answers to the tests in the order in which the tests are given in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤  2·10<sup class="upper-index">5</sup></span>) — the number of the test data.</p><p>Each of the next <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 1000</span>).</p>

## Output

<p>For each test from the input print the answer to the problem modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>. Print the answers to the tests in the order in which the tests are given in the input.</p>





```input1
6
1 1
2 1
2 2
3 1
3 2
3 3

```




```output1
1
3
0
6
2
0

```



## Note

<p>In the first test sample there is exactly one beautiful sequence: <span class="tex-span">(1, 1)</span>.</p><p>In the second test sample, the following sequences are beautiful: </p><ul> <li> <span class="tex-span">(1, 1)</span>; </li><li> <span class="tex-span">(1, 2)</span>; </li><li> <span class="tex-span">(2, 2)</span>. </li></ul><p>In the fourth test sample, the following sequences are beautiful: </p><ul> <li> <span class="tex-span">(1, 1)</span>; </li><li> <span class="tex-span">(1, 2)</span>; </li><li> <span class="tex-span">(1, 3)</span>; </li><li> <span class="tex-span">(2, 2)</span>; </li><li> <span class="tex-span">(2, 3)</span>; </li><li> <span class="tex-span">(3, 3)</span>. </li></ul><p>In the fifth test sample, the following sequences are beautiful: </p><ul> <li> <span class="tex-span">(1, 1), (2, 3)</span>; </li><li> <span class="tex-span">(1, 2), (3, 3)</span>. </li></ul><p>In the third and sixth samples, there are no beautiful sequences.</p>
