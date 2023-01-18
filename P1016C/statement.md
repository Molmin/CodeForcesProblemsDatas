## Description

<div><p>Vasya's house is situated in a forest, and there is a mushroom glade near it. The glade consists of two rows, each of which can be divided into <span class="tex-span"><i>n</i></span> consecutive cells. For each cell Vasya knows how fast the mushrooms grow in this cell (more formally, how many grams of mushrooms grow in this cell each minute). Vasya spends exactly one minute to move to some adjacent cell. Vasya cannot leave the glade. Two cells are considered adjacent if they share a common side. When Vasya enters some cell, he instantly collects all the mushrooms growing there.</p><p>Vasya begins his journey in the left upper cell. Every minute Vasya must move to some adjacent cell, he cannot wait for the mushrooms to grow. He wants to visit all the cells <span class="tex-font-style-bf">exactly once</span> and maximize the total weight of the collected mushrooms. Initially, all mushrooms have a weight of <span class="tex-span">0</span>. Note that Vasya doesn't need to return to the starting cell.</p><p>Help Vasya! Calculate the maximum total weight of mushrooms he can collect.</p></div><div class="input-specification"><p>The first line contains the number <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the length of the glade.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the growth rate of mushrooms in the first row of the glade.</p><p>The third line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> is the growth rate of mushrooms in the second row of the glade.</p></div><div class="output-specification"><p>Output one number — the maximum total weight of mushrooms that Vasya can collect by choosing the optimal route. Pay attention that Vasya must visit every cell of the glade <span class="tex-font-style-bf">exactly once</span>.</p></div>

## Input

<p>The first line contains the number <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the length of the glade.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> — the growth rate of mushrooms in the first row of the glade.</p><p>The third line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span> is the growth rate of mushrooms in the second row of the glade.</p>

## Output

<p>Output one number — the maximum total weight of mushrooms that Vasya can collect by choosing the optimal route. Pay attention that Vasya must visit every cell of the glade <span class="tex-font-style-bf">exactly once</span>.</p>





```input1
3
1 2 3
6 5 4

```




```input2
3
1 1000 10000
10 100 100000

```




```output1
70

```




```output2
543210

```



## Note

<p>In the first test case, the optimal route is as follows: </p><center> <img class="tex-graphics" src="file://jxhvsNEt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Thus, the collected weight of mushrooms will be <span class="tex-span">0·1 + 1·2 + 2·3 + 3·4 + 4·5 + 5·6 = 70</span>.<p>In the second test case, the optimal route is as follows: </p><center> <img class="tex-graphics" src="file://LAPhxI19.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> Thus, the collected weight of mushrooms will be <span class="tex-span">0·1 + 1·10 + 2·100 + 3·1000 + 4·10000 + 5·100000 = 543210</span>.
