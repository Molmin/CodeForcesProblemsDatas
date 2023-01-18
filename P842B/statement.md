## Description

<div><p>Gleb ordered pizza home. When the courier delivered the pizza, he was very upset, because several pieces of sausage lay on the crust, and he does not really like the crust.</p><p>The pizza is a circle of radius <span class="tex-span"><i>r</i></span> and center at the origin. Pizza consists of the main part — circle of radius <span class="tex-span"><i>r</i> - <i>d</i></span> with center at the origin, and crust around the main part of the width <span class="tex-span"><i>d</i></span>. Pieces of sausage are also circles. The radius of the <span class="tex-span"><i>i</i></span>&nbsp;-th piece of the sausage is <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, and the center is given as a pair (<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>).</p><p>Gleb asks you to help determine the number of pieces of sausage caught on the crust. A piece of sausage got on the crust, if it completely lies on the crust.</p></div><div class="input-specification"><p>First string contains two integer numbers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">0 ≤ <i>d</i> &lt; <i>r</i> ≤ 500</span>)&nbsp;— the radius of pizza and the width of crust.</p><p>Next line contains one integer number <span class="tex-span"><i>n</i></span>&nbsp;— the number of pieces of sausage (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains three integer numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 500 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>, <span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are coordinates of the center of <span class="tex-span"><i>i</i></span>-th peace of sausage, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— radius of <span class="tex-span"><i>i</i></span>-th peace of sausage.</p></div><div class="output-specification"><p>Output the number of pieces of sausage that lay on the crust.</p></div>

## Input

<p>First string contains two integer numbers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">0 ≤ <i>d</i> &lt; <i>r</i> ≤ 500</span>)&nbsp;— the radius of pizza and the width of crust.</p><p>Next line contains one integer number <span class="tex-span"><i>n</i></span>&nbsp;— the number of pieces of sausage (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Each of next <span class="tex-span"><i>n</i></span> lines contains three integer numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 500 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>, <span class="tex-span">0 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are coordinates of the center of <span class="tex-span"><i>i</i></span>-th peace of sausage, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— radius of <span class="tex-span"><i>i</i></span>-th peace of sausage.</p>

## Output

<p>Output the number of pieces of sausage that lay on the crust.</p>





```input1
8 4
7
7 8 1
-7 3 2
0 2 1
0 -2 2
-3 -3 1
0 6 2
5 3 1

```




```input2
10 8
4
0 0 9
0 0 10
1 0 1
1 0 2

```




```output1
2

```




```output2
0

```



## Note

<p>Below is a picture explaining the first example. Circles of green color denote pieces of sausage lying on the crust.</p><center> <img class="tex-graphics" src="file://gyKPQN2O.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
