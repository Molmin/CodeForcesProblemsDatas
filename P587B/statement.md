## Description

<div><p>While Duff was resting in the beach, she accidentally found a strange array <span class="tex-span"><i>b</i><sub class="lower-index">0</sub>, <i>b</i><sub class="lower-index">1</sub>, ..., <i>b</i><sub class="lower-index"><i>l</i> - 1</sub></span> consisting of <span class="tex-span"><i>l</i></span> positive integers. This array was strange because it was extremely long, but there was another (maybe shorter) array, <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> that <span class="tex-span"><i>b</i></span> can be build from <span class="tex-span"><i>a</i></span> with formula: <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i> <i>mod</i> <i>n</i></sub></span> where <span class="tex-span"><i>a</i> <i>mod</i> <i>b</i></span> denoted the remainder of dividing <span class="tex-span"><i>a</i></span> by <span class="tex-span"><i>b</i></span>.</p><center> <img class="tex-graphics" src="file://kU5aU0FS.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Duff is so curious, she wants to know the number of subsequences of <span class="tex-span"><i>b</i></span> like <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ..., <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>x</i></sub></sub></span> (<span class="tex-span">0 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>x</i></sub> &lt; <i>l</i></span>), such that: </p><ul> <li> <span class="tex-span">1 ≤ <i>x</i> ≤ <i>k</i></span> </li><li> For each <span class="tex-span">1 ≤ <i>j</i> ≤ <i>x</i> - 1</span>, <img align="middle" class="tex-formula" src="file://Ef3qgpEt.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> For each <span class="tex-span">1 ≤ <i>j</i> ≤ <i>x</i> - 1</span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>j</i></sub></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>j</i> + 1</sub></sub></span>. i.e this subsequence is non-decreasing. </li></ul><p>Since this number can be very large, she want to know it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Duff is not a programmer, and Malek is unavailable at the moment. So she asked for your help. Please tell her this number.</p></div><div class="input-specification"><p>The first line of input contains three integers, <span class="tex-span"><i>n</i>, <i>l</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i></span>, <span class="tex-span"><i>n</i> × <i>k</i> ≤ 10<sup class="upper-index">6</sup></span> and <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> for each <span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i> - 1</span>). </p></div><div class="output-specification"><p>Print the answer modulo <span class="tex-span">1 000 000 007</span> in one line.</p></div>

## Input

<p>The first line of input contains three integers, <span class="tex-span"><i>n</i>, <i>l</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i></span>, <span class="tex-span"><i>n</i> × <i>k</i> ≤ 10<sup class="upper-index">6</sup></span> and <span class="tex-span">1 ≤ <i>l</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">0</sub>, <i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> for each <span class="tex-span">0 ≤ <i>i</i> ≤ <i>n</i> - 1</span>). </p>

## Output

<p>Print the answer modulo <span class="tex-span">1 000 000 007</span> in one line.</p>





```input1
3 5 3
5 9 1

```




```input2
5 10 3
1 2 3 4 5

```




```output1
10

```




```output2
25

```



## Note

<p>In the first sample case, <img align="middle" class="tex-formula" src="file://k5JwDcjv.png" style="max-width: 100.0%;max-height: 100.0%;">. So all such sequences are: <img align="middle" class="tex-formula" src="file://YW1pGCaZ.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://xKqXZgyU.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://Lkdvudsa.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://OASxq0JK.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://4rscUixs.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://jcmDMjfS.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://h8zcwjUw.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://B3jJv8wg.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://BNjPmkJ0.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://tjPstaBV.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
