## Description

<div><p>Recently Duff has been a soldier in the army. Malek is her commander.</p><p>Their country, Andarz Gu has <span class="tex-span"><i>n</i></span> cities (numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>) and <span class="tex-span"><i>n</i> - 1</span> bidirectional roads. Each road connects two different cities. There exist a unique path between any two cities.</p><p>There are also <span class="tex-span"><i>m</i></span> people living in Andarz Gu (numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>). Each person has and ID number. ID number of <span class="tex-span"><i>i</i> - <i>th</i></span> person is <span class="tex-span"><i>i</i></span> and he/she lives in city number <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Note that there may be more than one person in a city, also there may be no people living in the city.</p><center> <img class="tex-graphics" src="file://EeVsFEcK.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Malek loves to order. That's why he asks Duff to answer to <span class="tex-span"><i>q</i></span> queries. In each query, he gives her numbers <span class="tex-span"><i>v</i>, <i>u</i></span> and <span class="tex-span"><i>a</i></span>.</p><p>To answer a query:</p><p>Assume there are <span class="tex-span"><i>x</i></span> people living in the cities lying on the path from city <span class="tex-span"><i>v</i></span> to city <span class="tex-span"><i>u</i></span>. Assume these people's IDs are <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>x</i></sub></span> in increasing order. </p><p>If <span class="tex-span"><i>k</i> = <i>min</i>(<i>x</i>, <i>a</i>)</span>, then Duff should tell Malek numbers <span class="tex-span"><i>k</i>, <i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> in this order. In the other words, Malek wants to know <span class="tex-span"><i>a</i></span> minimums on that path (or less, if there are less than <span class="tex-span"><i>a</i></span> people).</p><p>Duff is very busy at the moment, so she asked you to help her and answer the queries.</p></div><div class="input-specification"><p>The first line of input contains three integers, <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the roads. Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span>, endpoints of a road (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>).</p><p>Next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> separated by spaces (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>).</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the queries. Each of them contains three integers, <span class="tex-span"><i>v</i>, <i>u</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>a</i> ≤ 10</span>).</p></div><div class="output-specification"><p>For each query, print numbers <span class="tex-span"><i>k</i>, <i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> separated by spaces in one line.</p></div>

## Input

<p>The first line of input contains three integers, <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the roads. Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span>, endpoints of a road (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>).</p><p>Next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> separated by spaces (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> for each <span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>).</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the queries. Each of them contains three integers, <span class="tex-span"><i>v</i>, <i>u</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span> and <span class="tex-span">1 ≤ <i>a</i> ≤ 10</span>).</p>

## Output

<p>For each query, print numbers <span class="tex-span"><i>k</i>, <i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> separated by spaces in one line.</p>





```input1
5 4 5
1 3
1 2
1 4
4 5
2 1 4 3
4 5 6
1 5 2
5 5 10
2 3 3
5 3 1

```




```output1
1 3
2 2 3
0
3 1 2 4
1 2

```



## Note

<p>Graph of Andarz Gu in the sample case is as follows (ID of people in each city are written next to them):</p><center> <img class="tex-graphics" src="file://L7KoJczr.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
