## Description

<div><p>Everyone who has played Cut the Rope knows full well how the gameplay is organized. All levels in the game are divided into boxes. Initially only one box with some levels is available. Player should complete levels to earn stars, collecting stars opens new box with levels.</p><center> <img class="tex-graphics" src="file://E6tZriiO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Imagine that you are playing Cut the Rope for the first time. Currently you have only the levels of the first box (by the way, it is called "Cardboard Box"). Each level is characterized by two integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — how long it takes to complete the level for one star, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — how long it takes to complete the level for two stars <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>You want to open the next box as quickly as possible. So, you need to earn at least <span class="tex-span"><i>w</i></span> stars. How do make it happen? Note that the level can be passed only once: either for one star or for two. You do not necessarily need to pass all the levels.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>w</i> ≤ 2<i>n</i>)</span> — the number of levels in the first box and the number of stars you need to open another box. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the attributes of the <span class="tex-span"><i>i</i></span>-th level.</p></div><div class="output-specification"><p>In the first line print integer <span class="tex-span"><i>t</i></span> — the minimum time you need to open the next box. </p><p>In the next line, print <span class="tex-span"><i>n</i></span> digits without spaces — the description of the optimal scenario: </p><ul> <li> if you need to pass the <span class="tex-span"><i>i</i></span>-th level for one star, the <span class="tex-span"><i>i</i></span>-th digit should equal 1; </li><li> if you need to pass the <span class="tex-span"><i>i</i></span>-th level for two stars, the <span class="tex-span"><i>i</i></span>-th digit should equal 2; </li><li> if you do not need to pass the <span class="tex-span"><i>i</i></span>-th level at all, the <span class="tex-span"><i>i</i></span>-th digit should equal 0. </li></ul></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>w</i> ≤ 2<i>n</i>)</span> — the number of levels in the first box and the number of stars you need to open another box. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the attributes of the <span class="tex-span"><i>i</i></span>-th level.</p>

## Output

<p>In the first line print integer <span class="tex-span"><i>t</i></span> — the minimum time you need to open the next box. </p><p>In the next line, print <span class="tex-span"><i>n</i></span> digits without spaces — the description of the optimal scenario: </p><ul> <li> if you need to pass the <span class="tex-span"><i>i</i></span>-th level for one star, the <span class="tex-span"><i>i</i></span>-th digit should equal 1; </li><li> if you need to pass the <span class="tex-span"><i>i</i></span>-th level for two stars, the <span class="tex-span"><i>i</i></span>-th digit should equal 2; </li><li> if you do not need to pass the <span class="tex-span"><i>i</i></span>-th level at all, the <span class="tex-span"><i>i</i></span>-th digit should equal 0. </li></ul>





```input1
2 3
1 2
1 2

```




```input2
5 3
10 20
5 10
10 20
6 9
25 30

```




```output1
3
12

```




```output2
14
01020

```



## Note

<p>In the first test sample, answer <span class="tex-font-style-tt">21</span> is also assumed correct.</p>
