## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities in Berland, each of them has a unique id&nbsp;— an integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the capital is the one with id <span class="tex-span">1</span>. Now there is a serious problem in Berland with roads&nbsp;— there are no roads.</p><p>That is why there was a decision to build <span class="tex-span"><i>n</i> - 1</span> roads so that there will be exactly one simple path between each pair of cities.</p><p>In the construction plan <span class="tex-span"><i>t</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>t</i></sub></span> were stated, where <span class="tex-span"><i>t</i></span> equals to the distance from the capital to the most distant city, concerning new roads. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals the number of cities which should be at the distance <span class="tex-span"><i>i</i></span> from the capital. The distance between two cities is the number of roads one has to pass on the way from one city to another. </p><p>Also, it was decided that among all the cities except the capital there should be exactly <span class="tex-span"><i>k</i></span> cities with exactly one road going from each of them. Such cities are dead-ends and can't be economically attractive. In calculation of these cities the capital is not taken into consideration regardless of the number of roads from it. </p><p>Your task is to offer a plan of road's construction which satisfies all the described conditions or to inform that it is impossible.</p></div><div class="input-specification"><p>The first line contains three positive numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>t</i>, <i>k</i> &lt; <i>n</i></span>)&nbsp;— the distance to the most distant city from the capital and the number of cities which should be dead-ends (the capital in this number is not taken into consideration). </p><p>The second line contains a sequence of <span class="tex-span"><i>t</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>t</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), the <span class="tex-span"><i>i</i></span>-th number is the number of cities which should be at the distance <span class="tex-span"><i>i</i></span> from the capital. It is guaranteed that the sum of all the values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span"><i>n</i> - 1</span>.</p></div><div class="output-specification"><p>If it is impossible to built roads which satisfy all conditions, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of cities in Berland. In the each of the next <span class="tex-span"><i>n</i> - 1</span> line print two integers&nbsp;— the ids of cities that are connected by a road. Each road should be printed exactly once. You can print the roads and the cities connected by a road in any order.</p><p>If there are multiple answers, print any of them. Remember that the capital has id <span class="tex-span">1</span>.</p></div>

## Input

<p>The first line contains three positive numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>t</i>, <i>k</i> &lt; <i>n</i></span>)&nbsp;— the distance to the most distant city from the capital and the number of cities which should be dead-ends (the capital in this number is not taken into consideration). </p><p>The second line contains a sequence of <span class="tex-span"><i>t</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>t</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), the <span class="tex-span"><i>i</i></span>-th number is the number of cities which should be at the distance <span class="tex-span"><i>i</i></span> from the capital. It is guaranteed that the sum of all the values <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span"><i>n</i> - 1</span>.</p>

## Output

<p>If it is impossible to built roads which satisfy all conditions, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print one integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of cities in Berland. In the each of the next <span class="tex-span"><i>n</i> - 1</span> line print two integers&nbsp;— the ids of cities that are connected by a road. Each road should be printed exactly once. You can print the roads and the cities connected by a road in any order.</p><p>If there are multiple answers, print any of them. Remember that the capital has id <span class="tex-span">1</span>.</p>





```input1
7 3 3
2 3 1

```




```input2
14 5 6
4 4 2 2 1

```




```input3
3 1 1
2

```




```output1
7
1 3
2 1
2 6
2 4
7 4
3 5

```




```output2
14
3 1
1 4
11 6
1 2
10 13
6 10
10 12
14 12
8 4
5 1
3 7
2 6
5 9

```




```output3
-1

```


