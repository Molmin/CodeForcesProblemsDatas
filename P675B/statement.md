## Description

<div><p>Vasya works as a watchman in the gallery. Unfortunately, one of the most expensive paintings was stolen while he was on duty. He doesn't want to be fired, so he has to quickly restore the painting. He remembers some facts about it.</p><ul> <li> The painting is a square <span class="tex-span">3 × 3</span>, each cell contains a single integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and different cells may contain either different or equal integers. </li><li> The sum of integers in each of four squares <span class="tex-span">2 × 2</span> is equal to the sum of integers in the top left square <span class="tex-span">2 × 2</span>. </li><li> Four elements <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> are known and are located as shown on the picture below. </li></ul><center><img class="tex-graphics" src="file://i9zUzl4S.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Help Vasya find out the number of distinct squares the satisfy all the conditions above. Note, that this number may be equal to <span class="tex-span">0</span>, meaning Vasya remembers something wrong.</p><p>Two squares are considered to be different, if there exists a cell that contains two different integers in different squares.</p></div><div class="input-specification"><p>The first line of the input contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>)&nbsp;— maximum possible value of an integer in the cell and four integers that Vasya remembers.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of distinct valid squares.</p></div>

## Input

<p>The first line of the input contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>)&nbsp;— maximum possible value of an integer in the cell and four integers that Vasya remembers.</p>

## Output

<p>Print one integer&nbsp;— the number of distinct valid squares.</p>





```input1
2 1 1 1 2

```




```input2
3 3 1 2 3

```




```output1
2

```




```output2
6

```



## Note

<p>Below are all the possible paintings for the first sample. <img class="tex-graphics" src="file://g2g69koY.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://qxHnBb4j.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>In the second sample, only paintings displayed below satisfy all the rules. <img class="tex-graphics" src="file://J66Bq26f.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://4ozQXjDz.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://DVTEnstu.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://mYWooIZE.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://DdbZCbDO.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://R4Anw8KQ.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
