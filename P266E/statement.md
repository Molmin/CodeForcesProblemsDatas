## Description

<div><p>You've got an array, consisting of <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Your task is to quickly run the queries of two types:</p><ol><li> Assign value <span class="tex-span"><i>x</i></span> to all elements from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusive. After such query the values of the elements of array <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> become equal to <span class="tex-span"><i>x</i></span>.</li><li> Calculate and print sum <img align="middle" class="tex-formula" src="file://oi5ypOtD.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>k</i></span> doesn't exceed <span class="tex-span">5</span>. As the value of the sum can be rather large, you should print it modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</li></ol></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), showing, how many numbers are in the array and the number of queries, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the initial values of the array elements.</p><p>Then <span class="tex-span"><i>m</i></span> queries follow, one per line:</p><ol><li> The assign query has the following format: "<img align="middle" class="tex-formula" src="file://jpszx1Bf.png" style="max-width: 100.0%;max-height: 100.0%;">", (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</li><li> The query to calculate the sum has the following format: "<img align="middle" class="tex-formula" src="file://GKSiKWE8.png" style="max-width: 100.0%;max-height: 100.0%;">", (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;0 ≤ <i>k</i> ≤ 5</span>).</li></ol><p>All numbers in the input are integers.</p></div><div class="output-specification"><p>For each query to calculate the sum print an integer — the required sum modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>), showing, how many numbers are in the array and the number of queries, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the initial values of the array elements.</p><p>Then <span class="tex-span"><i>m</i></span> queries follow, one per line:</p><ol><li> The assign query has the following format: "<img align="middle" class="tex-formula" src="file://jpszx1Bf.png" style="max-width: 100.0%;max-height: 100.0%;">", (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</li><li> The query to calculate the sum has the following format: "<img align="middle" class="tex-formula" src="file://GKSiKWE8.png" style="max-width: 100.0%;max-height: 100.0%;">", (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;0 ≤ <i>k</i> ≤ 5</span>).</li></ol><p>All numbers in the input are integers.</p>

## Output

<p>For each query to calculate the sum print an integer — the required sum modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
4 5
5 10 2 1
? 1 2 1
= 2 2 0
? 2 4 3
= 1 4 1
? 1 4 5

```




```input2
3 1
1000000000 1000000000 1000000000
? 1 3 0

```




```output1
25
43
1300

```




```output2
999999986

```


