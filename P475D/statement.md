## Description

<div><p>Given a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>q</i></span> queries <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>q</i></sub></span> on it. For each query <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> you have to count the number of pairs <span class="tex-span">(<i>l</i>, <i>r</i>)</span> such that <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span> and <span class="tex-span"><i>gcd</i>(<i>a</i><sub class="lower-index"><i>l</i></sub>, <i>a</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>r</i></sub>) = <i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p><img align="middle" class="tex-formula" src="file://9gLrQJuZ.png" style="max-width: 100.0%;max-height: 100.0%;"> is a greatest common divisor of <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span>, that is equal to a largest positive integer that divides all <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span>, (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the length of the sequence. The next line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line of the input contains integer <span class="tex-span"><i>q</i></span>, (<span class="tex-span">1 ≤ <i>q</i> ≤ 3 × 10<sup class="upper-index">5</sup></span>), denoting the number of queries. Then follows <span class="tex-span"><i>q</i></span> lines, each contain an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>For each query print the result in a separate line.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span>, (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), denoting the length of the sequence. The next line contains <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line of the input contains integer <span class="tex-span"><i>q</i></span>, (<span class="tex-span">1 ≤ <i>q</i> ≤ 3 × 10<sup class="upper-index">5</sup></span>), denoting the number of queries. Then follows <span class="tex-span"><i>q</i></span> lines, each contain an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>For each query print the result in a separate line.</p>





```input1
3
2 6 3
5
1
2
3
4
6

```




```input2
7
10 20 3 15 1000 60 16
10
1
2
3
4
5
6
10
20
60
1000

```




```output1
1
2
2
0
1

```




```output2
14
0
2
2
2
0
2
2
1
1

```


