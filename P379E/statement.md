## Description

<div><p>Due to atheistic Soviet past, Christmas wasn't officially celebrated in Russia for most of the twentieth century. As a result, the Russian traditions for Christmas and New Year mixed into one event celebrated on the New Year but including the tree, a Santa-like 'Grandfather Frost', presents and huge family reunions and dinner parties all over the country. Bying a Tree at the New Year and installing it in the house is a tradition. Usually the whole family decorates the tree on the New Year Eve. We hope that Codeforces is a big and loving family, so in this problem we are going to decorate a tree as well.</p><p>So, our decoration consists of <span class="tex-span"><i>n</i></span> pieces, each piece is a piece of colored paper, its border is a closed polyline of a special shape. The pieces go one by one as is shown on the picture. The <span class="tex-span"><i>i</i></span>-th piece is a polyline that goes through points: <span class="tex-span">(0, 0)</span>, <span class="tex-span">(0, <i>y</i><sub class="lower-index">0</sub>)</span>, <span class="tex-span">(1, <i>y</i><sub class="lower-index">1</sub>)</span>, <span class="tex-span">(2, <i>y</i><sub class="lower-index">2</sub>)</span>, ..., <span class="tex-span">(<i>k</i>, <i>y</i><sub class="lower-index"><i>k</i></sub>)</span>, <span class="tex-span">(<i>k</i>, 0)</span>. The width of each piece equals <span class="tex-span"><i>k</i></span>.</p><center> <img class="tex-graphics" src="file://oBhK73D1.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script">The figure to the left shows the decoration, the figure to the right shows the individual pieces it consists of.</span> </center><p>The piece number 1 (shown red on the figure) is the outer piece (we see it completely), piece number 2 (shown yellow) follows it (we don't see it completely as it is partially closed by the first piece) and so on. The programmers are quite curious guys, so the moment we hung a decoration on the New Year tree we started to wonder: what area of each piece can people see?</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 300)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i> + 1</span> integers — the description of the polyline. If the <span class="tex-span"><i>i</i></span>-th line contains ontegers <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i>, 0</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>, ..., <i>y</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span>, that means that the polyline of the <span class="tex-span"><i>i</i></span>-th piece goes through points <span class="tex-span">(0, 0)</span>, <span class="tex-span">(0, <i>y</i><sub class="lower-index"><i>i</i>, 0</sub>)</span>, <span class="tex-span">(1, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>)</span>, <span class="tex-span">(2, <i>y</i><sub class="lower-index"><i>i</i>, 2</sub>)</span>, ..., <span class="tex-span">(<i>k</i>, <i>y</i><sub class="lower-index"><i>i</i>, <i>k</i></sub>)</span>, <span class="tex-span">(<i>k</i>, 0)</span> <span class="tex-span">(1 ≤ <i>y</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 1000)</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> real numbers — for each polyline, the area of its visible part.</p><p>The answer will be considered correct if its relative or absolute error do not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.  </p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 300)</span>. Each of the following <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>k</i> + 1</span> integers — the description of the polyline. If the <span class="tex-span"><i>i</i></span>-th line contains ontegers <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i>, 0</sub>, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>, ..., <i>y</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span>, that means that the polyline of the <span class="tex-span"><i>i</i></span>-th piece goes through points <span class="tex-span">(0, 0)</span>, <span class="tex-span">(0, <i>y</i><sub class="lower-index"><i>i</i>, 0</sub>)</span>, <span class="tex-span">(1, <i>y</i><sub class="lower-index"><i>i</i>, 1</sub>)</span>, <span class="tex-span">(2, <i>y</i><sub class="lower-index"><i>i</i>, 2</sub>)</span>, ..., <span class="tex-span">(<i>k</i>, <i>y</i><sub class="lower-index"><i>i</i>, <i>k</i></sub>)</span>, <span class="tex-span">(<i>k</i>, 0)</span> <span class="tex-span">(1 ≤ <i>y</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 1000)</span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> real numbers — for each polyline, the area of its visible part.</p><p>The answer will be considered correct if its relative or absolute error do not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.  </p>





```input1
2 2
2 1 2
1 2 1

```




```input2
1 1
1 1

```




```input3
4 1
2 7
7 2
5 5
6 4

```




```output1
3.000000000000
0.500000000000

```




```output2
1.000000000000

```




```output3
4.500000000000
1.250000000000
0.050000000000
0.016666666667

```


