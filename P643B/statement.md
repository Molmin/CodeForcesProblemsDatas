## Description

<div><p>Bearland has <span class="tex-span"><i>n</i></span> cities, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. Cities are connected via bidirectional roads. Each road connects two distinct cities. No two roads connect the same pair of cities.</p><p>Bear Limak was once in a city <span class="tex-span"><i>a</i></span> and he wanted to go to a city <span class="tex-span"><i>b</i></span>. There was no direct connection so he decided to take a long walk, visiting each city <span class="tex-font-style-bf">exactly once</span>. Formally: </p><ul> <li> There is no road between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. </li><li> There exists a sequence (path) of <span class="tex-span"><i>n</i></span> distinct cities <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> that <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = <i>a</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>n</i></sub> = <i>b</i></span> and there is a road between <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <img align="middle" class="tex-formula" src="file://G2fHEsrp.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>On the other day, the similar thing happened. Limak wanted to travel between a city <span class="tex-span"><i>c</i></span> and a city <span class="tex-span"><i>d</i></span>. There is no road between them but there exists a sequence of <span class="tex-span"><i>n</i></span> distinct cities <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub></span> that <span class="tex-span"><i>u</i><sub class="lower-index">1</sub> = <i>c</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>n</i></sub> = <i>d</i></span> and there is a road between <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i> + 1</sub></span> for <img align="middle" class="tex-formula" src="file://XBlMGjPG.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>Also, Limak thinks that there are at most <span class="tex-span"><i>k</i></span> roads in Bearland. He wonders whether he remembers everything correctly.</p><p>Given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and four distinct cities <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, can you find possible paths <span class="tex-span">(<i>v</i><sub class="lower-index">1</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub>)</span> and <span class="tex-span">(<i>u</i><sub class="lower-index">1</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub>)</span> to satisfy all the given conditions? Find any solution or print <span class="tex-font-style-tt">-1</span> if it's impossible.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>k</i> ≤ 2<i>n</i> - 2</span>)&nbsp;— the number of cities and the maximum allowed number of roads, respectively.</p><p>The second line contains four <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if it's impossible to satisfy all the given conditions. Otherwise, print two lines with paths descriptions. The first of these two lines should contain <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = <i>a</i></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>n</i></sub> = <i>b</i></span>. The second line should contain <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>u</i><sub class="lower-index">1</sub> = <i>c</i></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>n</i></sub> = <i>d</i></span>.</p><p>Two paths generate at most <span class="tex-span">2<i>n</i> - 2</span> roads: <span class="tex-span">(<i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>), (<i>v</i><sub class="lower-index">2</sub>, <i>v</i><sub class="lower-index">3</sub>), ..., (<i>v</i><sub class="lower-index"><i>n</i> - 1</sub>, <i>v</i><sub class="lower-index"><i>n</i></sub>), (<i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>), (<i>u</i><sub class="lower-index">2</sub>, <i>u</i><sub class="lower-index">3</sub>), ..., (<i>u</i><sub class="lower-index"><i>n</i> - 1</sub>, <i>u</i><sub class="lower-index"><i>n</i></sub>)</span>. Your answer will be considered wrong if contains more than <span class="tex-span"><i>k</i></span> distinct roads or any other condition breaks. Note that <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and <span class="tex-span">(<i>y</i>, <i>x</i>)</span> are the same road.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>k</i> ≤ 2<i>n</i> - 2</span>)&nbsp;— the number of cities and the maximum allowed number of roads, respectively.</p><p>The second line contains four <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if it's impossible to satisfy all the given conditions. Otherwise, print two lines with paths descriptions. The first of these two lines should contain <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> = <i>a</i></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>n</i></sub> = <i>b</i></span>. The second line should contain <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub></span> where <span class="tex-span"><i>u</i><sub class="lower-index">1</sub> = <i>c</i></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>n</i></sub> = <i>d</i></span>.</p><p>Two paths generate at most <span class="tex-span">2<i>n</i> - 2</span> roads: <span class="tex-span">(<i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>), (<i>v</i><sub class="lower-index">2</sub>, <i>v</i><sub class="lower-index">3</sub>), ..., (<i>v</i><sub class="lower-index"><i>n</i> - 1</sub>, <i>v</i><sub class="lower-index"><i>n</i></sub>), (<i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>), (<i>u</i><sub class="lower-index">2</sub>, <i>u</i><sub class="lower-index">3</sub>), ..., (<i>u</i><sub class="lower-index"><i>n</i> - 1</sub>, <i>u</i><sub class="lower-index"><i>n</i></sub>)</span>. Your answer will be considered wrong if contains more than <span class="tex-span"><i>k</i></span> distinct roads or any other condition breaks. Note that <span class="tex-span">(<i>x</i>, <i>y</i>)</span> and <span class="tex-span">(<i>y</i>, <i>x</i>)</span> are the same road.</p>





```input1
7 11
2 4 7 3

```




```input2
1000 999
10 20 30 40

```




```output1
2 7 1 3 6 5 4
7 1 5 4 6 2 3

```




```output2
-1

```



## Note

<p>In the first sample test, there should be <span class="tex-span">7</span> cities and at most <span class="tex-span">11</span> roads. The provided sample solution generates <span class="tex-span">10</span> roads, as in the drawing. You can also see a simple path of length <span class="tex-span"><i>n</i></span> between <span class="tex-span">2</span> and <span class="tex-span">4</span>, and a path between <span class="tex-span">7</span> and <span class="tex-span">3</span>.</p><center> <img class="tex-graphics" src="file://XD3tRzL0.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
