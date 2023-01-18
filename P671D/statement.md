## Description

<div><p>Mayor of Yusland just won the lottery and decided to spent money on something good for town. For example, repair all the roads in the town.</p><p>Yusland consists of <span class="tex-span"><i>n</i></span> intersections connected by <span class="tex-span"><i>n</i> - 1</span> bidirectional roads. One can travel from any intersection to any other intersection using only these roads.</p><p>There is only one road repairing company in town, named "RC company". Company's center is located at the intersection <span class="tex-span">1</span>. RC company doesn't repair roads you tell them. Instead, they have workers at some intersections, who can repair only some specific paths. The <span class="tex-span"><i>i</i></span>-th worker can be paid <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> coins and then he repairs <span class="tex-font-style-bf">all roads</span> on a path from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to some <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> that <span class="tex-font-style-bf">lies on the path</span> from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to intersection <span class="tex-span">1</span>. </p><p>Mayor asks you to choose the cheapest way to hire some subset of workers in order to repair all the roads in Yusland. It's allowed that some roads will be repaired more than once.</p><p>If it's impossible to repair all roads print <span class="tex-span"> - 1</span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300 000</span>)&nbsp;— the number of cities in Yusland and the number of workers respectively.</p><p>Then follow <span class="tex-span"><i>n</i>−1</span> line, each of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of intersections connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>Last <span class="tex-span"><i>m</i></span> lines provide the description of workers, each line containing three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). This means that the <span class="tex-span"><i>i</i></span>-th worker can repair all roads on the path from <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> coins. It's guaranteed that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> lies on the path from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span">1</span>. Note that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> may coincide.</p></div><div class="output-specification"><p>If it's impossible to repair all roads then print <span class="tex-span"> - 1</span>. Otherwise print a single integer&nbsp;— minimum cost required to repair all roads using "RC company" workers.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300 000</span>)&nbsp;— the number of cities in Yusland and the number of workers respectively.</p><p>Then follow <span class="tex-span"><i>n</i>−1</span> line, each of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— indices of intersections connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>Last <span class="tex-span"><i>m</i></span> lines provide the description of workers, each line containing three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). This means that the <span class="tex-span"><i>i</i></span>-th worker can repair all roads on the path from <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> coins. It's guaranteed that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> lies on the path from <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span">1</span>. Note that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> may coincide.</p>

## Output

<p>If it's impossible to repair all roads then print <span class="tex-span"> - 1</span>. Otherwise print a single integer&nbsp;— minimum cost required to repair all roads using "RC company" workers.</p>





```input1
6 5
1 2
1 3
3 4
4 5
4 6
2 1 2
3 1 4
4 1 3
5 3 1
6 3 2

```




```output1
8

```



## Note

<p>In the first sample, we should choose workers with indices <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span>, some roads will be repaired more than once but it is OK. The cost will be equal to <span class="tex-span">2 + 3 + 1 + 2 = 8</span> coins.</p>
