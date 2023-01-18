## Description

<div><p>Vasya follows a basketball game and marks the distances from which each team makes a throw. He knows that each successful throw has value of either 2 or 3 points. A throw is worth 2 points if the distance it was made from doesn't exceed some value of <span class="tex-span"><i>d</i></span> meters, and a throw is worth 3 points if the distance is larger than <span class="tex-span"><i>d</i></span> meters, where <span class="tex-span"><i>d</i></span> is some <span class="tex-font-style-bf">non-negative</span> integer.</p><p>Vasya would like the advantage of the points scored by the first team (the points of the first team minus the points of the second team) to be maximum. For that he can mentally choose the value of <span class="tex-span"><i>d</i></span>. Help him to do that.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of throws of the first team. Then follow <span class="tex-span"><i>n</i></span> integer numbers — the distances of throws <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>). </p><p>Then follows number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of the throws of the second team. Then follow <span class="tex-span"><i>m</i></span> integer numbers — the distances of throws of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print two numbers in the format <span class="tex-font-style-tt">a:b</span> — the score that is possible considering the problem conditions where the result of subtraction <span class="tex-span"><i>a</i> - <i>b</i></span> is maximum. If there are several such scores, find the one in which number <span class="tex-span"><i>a</i></span> is maximum.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of throws of the first team. Then follow <span class="tex-span"><i>n</i></span> integer numbers — the distances of throws <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>). </p><p>Then follows number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of the throws of the second team. Then follow <span class="tex-span"><i>m</i></span> integer numbers — the distances of throws of <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print two numbers in the format <span class="tex-font-style-tt">a:b</span> — the score that is possible considering the problem conditions where the result of subtraction <span class="tex-span"><i>a</i> - <i>b</i></span> is maximum. If there are several such scores, find the one in which number <span class="tex-span"><i>a</i></span> is maximum.</p>





```input1
3
1 2 3
2
5 6

```




```input2
5
6 7 8 9 10
5
1 2 3 4 5

```




```output1
9:6

```




```output2
15:10

```


