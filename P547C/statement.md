## Description

<div><p>Mike is a bartender at Rico's bar. At Rico's, they put beer glasses in a special shelf. There are <span class="tex-span"><i>n</i></span> kinds of beer at Rico's numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. <span class="tex-span"><i>i</i></span>-th kind of beer has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> milliliters of foam on it.</p><center> <img class="tex-graphics" src="file://ipWS2C9j.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Maxim is Mike's boss. Today he told Mike to perform <span class="tex-span"><i>q</i></span> queries. Initially the shelf is empty. In each request, Maxim gives him a number <span class="tex-span"><i>x</i></span>. If beer number <span class="tex-span"><i>x</i></span> is already in the shelf, then Mike should remove it from the shelf, otherwise he should put it in the shelf.</p><p>After each query, Mike should tell him the score of the shelf. Bears are geeks. So they think that the score of a shelf is the number of pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> of glasses in the shelf such that <span class="tex-span"><i>i</i> &lt; <i>j</i></span> and <img align="middle" class="tex-formula" src="file://pLmhW3P4.png" style="max-width: 100.0%;max-height: 100.0%;"> where <img align="middle" class="tex-formula" src="file://QSwt3tbs.png" style="max-width: 100.0%;max-height: 100.0%;"> is the greatest common divisor of numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>Mike is tired. So he asked you to help him in performing these requests.</p></div><div class="input-specification"><p>The first line of input contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>), the number of different kinds of beer and number of queries.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5 × 10<sup class="upper-index">5</sup></span>), the height of foam in top of each kind of beer.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the queries. Each query consists of a single integer integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), the index of a beer that should be added or removed from the shelf.</p></div><div class="output-specification"><p>For each query, print the answer for that query in one line.</p></div>

## Input

<p>The first line of input contains numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 2 × 10<sup class="upper-index">5</sup></span>), the number of different kinds of beer and number of queries.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space separated integers, <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5 × 10<sup class="upper-index">5</sup></span>), the height of foam in top of each kind of beer.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the queries. Each query consists of a single integer integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), the index of a beer that should be added or removed from the shelf.</p>

## Output

<p>For each query, print the answer for that query in one line.</p>





```input1
5 6
1 2 3 4 6
1
2
3
4
5
1

```




```output1
0
1
3
5
6
2

```


