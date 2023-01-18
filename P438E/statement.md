## Description

<div><p>Our child likes computer science very much, especially he likes binary trees.</p><p>Consider the sequence of <span class="tex-span"><i>n</i></span> distinct positive integers: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>. The child calls a vertex-weighted rooted binary tree <span class="tex-font-style-it">good</span> if and only if for every vertex <span class="tex-span"><i>v</i></span>, the weight of <span class="tex-span"><i>v</i></span> is in the set <span class="tex-span">{<i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub>}</span>. Also our child thinks that the <span class="tex-font-style-it">weight</span> of a vertex-weighted tree is the sum of all vertices' weights.</p><p>Given an integer <span class="tex-span"><i>m</i></span>, can you for all <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ <i>s</i> ≤ <i>m</i>)</span> calculate the number of good vertex-weighted rooted binary trees with weight <span class="tex-span"><i>s</i></span>? Please, check the samples for better understanding what trees are considered different.</p><p>We only want to know the answer modulo <span class="tex-span">998244353</span> (<span class="tex-span">7 × 17 × 2<sup class="upper-index">23</sup> + 1</span>, a prime number).</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated pairwise distinct integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>. <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, each line containing a single integer. The <span class="tex-span"><i>i</i></span>-th line must contain the number of good vertex-weighted rooted binary trees whose weight exactly equal to <span class="tex-span"><i>i</i></span>. Print the answers modulo <span class="tex-span">998244353</span> (<span class="tex-span">7 × 17 × 2<sup class="upper-index">23</sup> + 1</span>, a prime number).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated pairwise distinct integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span>. <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, each line containing a single integer. The <span class="tex-span"><i>i</i></span>-th line must contain the number of good vertex-weighted rooted binary trees whose weight exactly equal to <span class="tex-span"><i>i</i></span>. Print the answers modulo <span class="tex-span">998244353</span> (<span class="tex-span">7 × 17 × 2<sup class="upper-index">23</sup> + 1</span>, a prime number).</p>





```input1
2 3
1 2

```




```input2
3 10
9 4 3

```




```input3
5 10
13 10 6 4 15

```




```output1
1
3
9

```




```output2
0
0
1
1
0
2
4
2
6
15

```




```output3
0
0
0
1
0
1
0
2
0
5

```



## Note

<p>In the first example, there are <span class="tex-span">9</span> good vertex-weighted rooted binary trees whose weight exactly equal to <span class="tex-span">3</span>:</p><center> <img class="tex-graphics" src="file://WoeokUei.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
