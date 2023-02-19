## Description

<div><p>Young Timofey has a birthday today! He got kit of <span class="tex-span"><i>n</i></span> cubes as a birthday present from his parents. Every cube has a number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, which is written on it. Timofey put all the cubes in a row and went to unpack other presents.</p><p>In this time, Timofey's elder brother, Dima reordered the cubes using the following rule. Suppose the cubes are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in their order. Dima performs several steps, on step <span class="tex-span"><i>i</i></span> he reverses the segment of cubes from <span class="tex-span"><i>i</i></span>-th to <span class="tex-span">(<i>n</i> - <i>i</i> + 1)</span>-th. He does this while <span class="tex-span"><i>i</i> ≤ <i>n</i> - <i>i</i> + 1</span>.</p><p>After performing the operations Dima went away, being very proud of himself. When Timofey returned to his cubes, he understood that their order was changed. Help Timofey as fast as you can and save the holiday&nbsp;— restore the initial order of the cubes using information of their current location.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cubes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number written on the <span class="tex-span"><i>i</i></span>-th cube after Dima has changed their order.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers, separated by spaces&nbsp;— the numbers written on the cubes in their initial order.</p><p>It can be shown that the answer is unique.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cubes.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number written on the <span class="tex-span"><i>i</i></span>-th cube after Dima has changed their order.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers, separated by spaces&nbsp;— the numbers written on the cubes in their initial order.</p><p>It can be shown that the answer is unique.</p>





```input1
7
4 3 7 6 9 1 2

```




```input2
8
6 1 4 2 5 6 9 2

```




```output1
2 3 9 6 7 1 4
```




```output2
2 1 6 2 5 4 9 6
```



## Note

<p>Consider the first sample.</p><ol> <li> At the begining row was [<span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">9</span>, <span class="tex-span">6</span>, <span class="tex-span">7</span>, <span class="tex-span">1</span>, <span class="tex-span">4</span>]. </li><li> After first operation row was [<span class="tex-span">4</span>, <span class="tex-span">1</span>, <span class="tex-span">7</span>, <span class="tex-span">6</span>, <span class="tex-span">9</span>, <span class="tex-span">3</span>, <span class="tex-span">2</span>]. </li><li> After second operation row was [<span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">9</span>, <span class="tex-span">6</span>, <span class="tex-span">7</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>]. </li><li> After third operation row was [<span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">7</span>, <span class="tex-span">6</span>, <span class="tex-span">9</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>]. </li><li> At fourth operation we reverse just middle element, so nothing has changed. The final row is [<span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">7</span>, <span class="tex-span">6</span>, <span class="tex-span">9</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span>]. So the answer for this case is row [<span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">9</span>, <span class="tex-span">6</span>, <span class="tex-span">7</span>, <span class="tex-span">1</span>, <span class="tex-span">4</span>]. </li></ol>
