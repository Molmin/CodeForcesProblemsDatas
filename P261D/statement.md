## Description

<div><p>Maxim loves sequences, especially those that strictly increase. He is wondering, what is the length of the longest increasing subsequence of the given sequence <span class="tex-span"><i>a</i></span>?</p><p>Sequence <span class="tex-span"><i>a</i></span> is given as follows: </p><ul> <li> the length of the sequence equals <span class="tex-span"><i>n</i> × <i>t</i></span>; </li><li> <img align="middle" class="tex-formula" src="file://DgEt6bXW.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i> × <i>t</i>)</span>, where operation <img align="middle" class="tex-formula" src="file://23dOS9af.png" style="max-width: 100.0%;max-height: 100.0%;"> means taking the remainder after dividing number <span class="tex-span"><i>x</i></span> by number <span class="tex-span"><i>y</i></span>. </li></ul><p>Sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>,  <i>s</i><sub class="lower-index">2</sub>,  ...,  <i>s</i><sub class="lower-index"><i>r</i></sub></span> of length <span class="tex-span"><i>r</i></span> is a <span class="tex-font-style-it">subsequence</span> of sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span>, if there is such increasing sequence of indexes <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>r</i></sub></span> <span class="tex-span">(1  ≤  <i>i</i><sub class="lower-index">1</sub>  &lt;  <i>i</i><sub class="lower-index">2</sub>  &lt; ...   &lt;  <i>i</i><sub class="lower-index"><i>r</i></sub>  ≤  <i>n</i>)</span>, that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>j</i></sub></sub>  =  <i>s</i><sub class="lower-index"><i>j</i></sub></span>. In other words, the subsequence can be obtained from the sequence by crossing out some elements.</p><p>Sequence <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>,  <i>s</i><sub class="lower-index">2</sub>,  ...,  <i>s</i><sub class="lower-index"><i>r</i></sub></span> is <span class="tex-font-style-it">increasing</span>, if the following inequality holds: <span class="tex-span"><i>s</i><sub class="lower-index">1</sub> &lt; <i>s</i><sub class="lower-index">2</sub> &lt;  ... &lt;  <i>s</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>Maxim have <span class="tex-span"><i>k</i></span> variants of the sequence <span class="tex-span"><i>a</i></span>. Help Maxim to determine for each sequence the length of the longest increasing subsequence.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>maxb</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10;&nbsp;1 ≤ <i>n</i>, <i>maxb</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>n</i> × <i>maxb</i> ≤ 2·10<sup class="upper-index">7</sup>)</span>. Each of the next <span class="tex-span"><i>k</i></span> lines contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>maxb</i>)</span>. </p><p>Note that for each variant of the sequence <span class="tex-span"><i>a</i></span> the values <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>maxb</i></span> and <span class="tex-span"><i>t</i></span> coincide, the only arrays <span class="tex-span"><i>b</i></span>s differ.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> integers — the answers for the variants of the sequence <span class="tex-span"><i>a</i></span>. Print the answers in the order the variants follow in the input.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>maxb</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10;&nbsp;1 ≤ <i>n</i>, <i>maxb</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;<i>n</i> × <i>maxb</i> ≤ 2·10<sup class="upper-index">7</sup>)</span>. Each of the next <span class="tex-span"><i>k</i></span> lines contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>maxb</i>)</span>. </p><p>Note that for each variant of the sequence <span class="tex-span"><i>a</i></span> the values <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>maxb</i></span> and <span class="tex-span"><i>t</i></span> coincide, the only arrays <span class="tex-span"><i>b</i></span>s differ.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> integers — the answers for the variants of the sequence <span class="tex-span"><i>a</i></span>. Print the answers in the order the variants follow in the input.</p>





```input1
3 3 5 2
3 2 1
1 2 3
2 3 1

```




```output1
2
3
3

```


