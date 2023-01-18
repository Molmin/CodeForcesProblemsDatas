## Description

<div><p>Vasya takes part in the orienteering competition. There are <span class="tex-span"><i>n</i></span> checkpoints located along the line at coordinates <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. Vasya starts at the point with coordinate <span class="tex-span"><i>a</i></span>. His goal is to visit at least <span class="tex-span"><i>n</i> - 1</span> checkpoint in order to finish the competition. Participant are allowed to visit checkpoints in arbitrary order.</p><p>Vasya wants to pick such checkpoints and the order of visiting them that the total distance travelled is minimized. He asks you to calculate this minimum possible value.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span"> - 1 000 000 ≤ <i>a</i> ≤ 1 000 000</span>)&nbsp;— the number of checkpoints and Vasya's starting position respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 1 000 000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— coordinates of the checkpoints.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum distance Vasya has to travel in order to visit at least <span class="tex-span"><i>n</i> - 1</span> checkpoint.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span"> - 1 000 000 ≤ <i>a</i> ≤ 1 000 000</span>)&nbsp;— the number of checkpoints and Vasya's starting position respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 1 000 000 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— coordinates of the checkpoints.</p>

## Output

<p>Print one integer&nbsp;— the minimum distance Vasya has to travel in order to visit at least <span class="tex-span"><i>n</i> - 1</span> checkpoint.</p>





```input1
3 10
1 7 12

```




```input2
2 0
11 -10

```




```input3
5 0
0 0 1000 0 0

```




```output1
7

```




```output2
10

```




```output3
0

```



## Note

<p>In the first sample Vasya has to visit at least two checkpoints. The optimal way to achieve this is the walk to the third checkpoints (distance is <span class="tex-span">12 - 10 = 2</span>) and then proceed to the second one (distance is <span class="tex-span">12 - 7 = 5</span>). The total distance is equal to <span class="tex-span">2 + 5 = 7</span>.</p><p>In the second sample it's enough to visit only one checkpoint so Vasya should just walk to the point <span class="tex-span"> - 10</span>.</p>
