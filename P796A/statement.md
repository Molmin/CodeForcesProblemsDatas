## Description

<div><p>Zane the wizard had never loved anyone before, until he fell in love with a girl, whose name remains unknown to us.</p><center> <img class="tex-graphics" src="file://zC3UF1EK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The girl lives in house <span class="tex-span"><i>m</i></span> of a village. There are <span class="tex-span"><i>n</i></span> houses in that village, lining in a straight line from left to right: house <span class="tex-span">1</span>, house <span class="tex-span">2</span>, ..., house <span class="tex-span"><i>n</i></span>. The village is also well-structured: house <span class="tex-span"><i>i</i></span> and house <span class="tex-span"><i>i</i> + 1</span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>) are exactly <span class="tex-span">10</span> meters away. In this village, some houses are occupied, and some are not. Indeed, unoccupied houses can be purchased.</p><p>You will be given <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> that denote the availability and the prices of the houses. If house <span class="tex-span"><i>i</i></span> is occupied, and therefore cannot be bought, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">0</span>. Otherwise, house <span class="tex-span"><i>i</i></span> can be bought, and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the money required to buy it, in dollars.</p><p>As Zane has only <span class="tex-span"><i>k</i></span> dollars to spare, it becomes a challenge for him to choose the house to purchase, so that he could live as near as possible to his crush. Help Zane determine the minimum distance from his crush's house to some house he can afford, to help him succeed in his love.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>)&nbsp;— the number of houses in the village, the house where the girl lives, and the amount of money Zane has (in dollars), respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— denoting the availability and the prices of the houses.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>m</i></sub> = 0</span> and that it is possible to purchase some house with no more than <span class="tex-span"><i>k</i></span> dollars.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the minimum distance, in meters, from the house where the girl Zane likes lives to the house Zane can buy.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>)&nbsp;— the number of houses in the village, the house where the girl lives, and the amount of money Zane has (in dollars), respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— denoting the availability and the prices of the houses.</p><p>It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>m</i></sub> = 0</span> and that it is possible to purchase some house with no more than <span class="tex-span"><i>k</i></span> dollars.</p>

## Output

<p>Print one integer&nbsp;— the minimum distance, in meters, from the house where the girl Zane likes lives to the house Zane can buy.</p>





```input1
5 1 20
0 27 32 21 19

```




```input2
7 3 50
62 0 0 0 99 33 22

```




```input3
10 5 100
1 0 1 0 0 0 0 0 1 1

```




```output1
40
```




```output2
30
```




```output3
20
```



## Note

<p>In the first sample, with <span class="tex-span"><i>k</i> = 20</span> dollars, Zane can buy only house <span class="tex-span">5</span>. The distance from house <span class="tex-span"><i>m</i> = 1</span> to house <span class="tex-span">5</span> is <span class="tex-span">10 + 10 + 10 + 10 = 40</span> meters.</p><p>In the second sample, Zane can buy houses <span class="tex-span">6</span> and <span class="tex-span">7</span>. It is better to buy house <span class="tex-span">6</span> than house <span class="tex-span">7</span>, since house <span class="tex-span"><i>m</i> = 3</span> and house <span class="tex-span">6</span> are only <span class="tex-span">30</span> meters away, while house <span class="tex-span"><i>m</i> = 3</span> and house <span class="tex-span">7</span> are <span class="tex-span">40</span> meters away.</p>
