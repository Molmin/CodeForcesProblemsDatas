## Description

<div><p>Simon has an array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> positive integers. Today Simon asked you to find a pair of integers <span class="tex-span"><i>l</i>, <i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>, such that the following conditions hold:</p><ol> <li> there is integer <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>l</i> ≤ <i>j</i> ≤ <i>r</i></span>), such that all integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub></span> are divisible by <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>; </li><li> value <span class="tex-span"><i>r</i> - <i>l</i></span> takes the maximum value among all pairs for which condition <span class="tex-span">1</span> is true; </li></ol><p>Help Simon, find the required pair of numbers <span class="tex-span">(<i>l</i>, <i>r</i>)</span>. If there are multiple required pairs find all of them.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>Print two integers in the first line — the number of required pairs and the maximum value of <span class="tex-span"><i>r</i> - <i>l</i></span>. On the following line print all <span class="tex-span"><i>l</i></span> values from optimal pairs in increasing order.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>Print two integers in the first line — the number of required pairs and the maximum value of <span class="tex-span"><i>r</i> - <i>l</i></span>. On the following line print all <span class="tex-span"><i>l</i></span> values from optimal pairs in increasing order.</p>





```input1
5
4 6 9 3 6

```




```input2
5
1 3 5 7 9

```




```input3
5
2 3 5 7 11

```




```output1
1 3
2 

```




```output2
1 4
1 

```




```output3
5 0
1 2 3 4 5 

```



## Note

<p>In the first sample the pair of numbers is right, as numbers <span class="tex-span">6, 9, 3</span> are divisible by <span class="tex-span">3</span>.</p><p>In the second sample all numbers are divisible by number <span class="tex-span">1</span>.</p><p>In the third sample all numbers are prime, so conditions <span class="tex-span">1</span> and <span class="tex-span">2</span> are true only for pairs of numbers <span class="tex-span">(1, 1)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(3, 3)</span>, <span class="tex-span">(4, 4)</span>, <span class="tex-span">(5, 5)</span>.</p>
