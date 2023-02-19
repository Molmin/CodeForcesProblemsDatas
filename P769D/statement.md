## Description

<div><p>Vasya has the sequence consisting of <span class="tex-span"><i>n</i></span> integers. Vasya consider the pair of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-font-style-it">k-interesting</span>, if their binary representation differs from each other exactly in <span class="tex-span"><i>k</i></span> bits. For example, if <span class="tex-span"><i>k</i> = 2</span>, the pair of integers <span class="tex-span"><i>x</i> = 5</span> and <span class="tex-span"><i>y</i> = 3</span> is <span class="tex-font-style-it">k-interesting</span>, because their binary representation <span class="tex-span"><i>x</i></span>=<span class="tex-font-style-tt">101</span> and <span class="tex-span"><i>y</i></span>=<span class="tex-font-style-tt">011</span> differs exactly in two bits.</p><p>Vasya wants to know how many pairs of indexes (<span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>) are in his sequence so that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and the pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is <span class="tex-font-style-it">k-interesting</span>. Your task is to help Vasya and determine this number.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 14</span>) — the number of integers in Vasya's sequence and the number of bits in which integers in <span class="tex-font-style-it">k-interesting</span> pair should differ.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), which Vasya has.</p></div><div class="output-specification"><p>Print the number of pairs (<span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>) so that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and the pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is <span class="tex-font-style-it">k-interesting</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 14</span>) — the number of integers in Vasya's sequence and the number of bits in which integers in <span class="tex-font-style-it">k-interesting</span> pair should differ.</p><p>The second line contains the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), which Vasya has.</p>

## Output

<p>Print the number of pairs (<span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>) so that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and the pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is <span class="tex-font-style-it">k-interesting</span>.</p>





```input1
4 1
0 3 2 1

```




```input2
6 0
200 100 100 100 200 200

```




```output1
4

```




```output2
6

```



## Note

<p>In the first test there are 4 <span class="tex-font-style-it">k-interesting</span> pairs:</p><ul> <li> (<span class="tex-span">1</span>, <span class="tex-span">3</span>), </li><li> (<span class="tex-span">1</span>, <span class="tex-span">4</span>), </li><li> (<span class="tex-span">2</span>, <span class="tex-span">3</span>), </li><li> (<span class="tex-span">2</span>, <span class="tex-span">4</span>). </li></ul><p>In the second test <span class="tex-span"><i>k</i> = 0</span>. Consequently, integers in any <span class="tex-font-style-it">k-interesting</span> pair should be equal to themselves. Thus, for the second test there are 6 <span class="tex-font-style-it">k-interesting</span> pairs:</p><ul> <li> (<span class="tex-span">1</span>, <span class="tex-span">5</span>), </li><li> (<span class="tex-span">1</span>, <span class="tex-span">6</span>), </li><li> (<span class="tex-span">2</span>, <span class="tex-span">3</span>), </li><li> (<span class="tex-span">2</span>, <span class="tex-span">4</span>), </li><li> (<span class="tex-span">3</span>, <span class="tex-span">4</span>), </li><li> (<span class="tex-span">5</span>, <span class="tex-span">6</span>). </li></ul>
