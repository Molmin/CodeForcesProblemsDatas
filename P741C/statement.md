## Description

<div><p><span class="tex-font-style-it">Note that girls in Arpa’s land are really attractive.</span></p><p>Arpa loves overnight parties. In the middle of one of these parties Mehrdad suddenly appeared. He saw <span class="tex-span"><i>n</i></span> pairs of friends sitting around a table. <span class="tex-span"><i>i</i></span>-th pair consisted of a boy, sitting on the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th chair, and his girlfriend, sitting on the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th chair. The chairs were numbered <span class="tex-span">1</span> through <span class="tex-span">2<i>n</i></span> in clockwise direction. There was exactly one person sitting on each chair.</p><center> <img class="tex-graphics" height="222px" src="file://UmrdXNuT.png" style="max-width: 100.0%;max-height: 100.0%;" width="213px"> </center><p>There were two types of food: Kooft and Zahre-mar. Now Mehrdad wonders, was there any way to serve food for the guests such that: </p><ul> <li> Each person had exactly one type of food, </li><li> No boy had the same type of food as his girlfriend, </li><li> Among any three guests sitting on consecutive chairs, there was two of them who had different type of food. Note that chairs <span class="tex-span">2<i>n</i></span> and <span class="tex-span">1</span> are considered consecutive. </li></ul><p>Find the answer for the Mehrdad question. If it was possible, find some arrangement of food types that satisfies the conditions.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  10<sup class="upper-index">5</sup></span>)&nbsp;— the number of pairs of guests.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤  2<i>n</i></span>)&nbsp;— the number of chair on which the boy in the <span class="tex-span"><i>i</i></span>-th pair was sitting and the number of chair on which his girlfriend was sitting. It's guaranteed that there was exactly one person sitting on each chair. </p></div><div class="output-specification"><p>If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain two integers which represent the type of food for the <span class="tex-span"><i>i</i></span>-th pair. The first integer in the line is the type of food the boy had, and the second integer is the type of food the girl had. If someone had Kooft, print <span class="tex-span">1</span>, otherwise print <span class="tex-span">2</span>.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  10<sup class="upper-index">5</sup></span>)&nbsp;— the number of pairs of guests.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1  ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤  2<i>n</i></span>)&nbsp;— the number of chair on which the boy in the <span class="tex-span"><i>i</i></span>-th pair was sitting and the number of chair on which his girlfriend was sitting. It's guaranteed that there was exactly one person sitting on each chair. </p>

## Output

<p>If there is no solution, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise print <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th of them should contain two integers which represent the type of food for the <span class="tex-span"><i>i</i></span>-th pair. The first integer in the line is the type of food the boy had, and the second integer is the type of food the girl had. If someone had Kooft, print <span class="tex-span">1</span>, otherwise print <span class="tex-span">2</span>.</p><p>If there are multiple solutions, print any of them.</p>





```input1
3
1 4
2 5
3 6

```




```output1
1 2
2 1
1 2

```


