## Description

<div><p>The country has <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>n</i> - 1</span> bidirectional roads, it is possible to get from every city to any other one if you move only along the roads. The cities are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive.</p><p>All the roads are initially bad, but the government wants to improve the state of some roads. We will assume that the citizens are happy about road improvement if the path from the capital located in city <span class="tex-span"><i>x</i></span> to any other city contains at most one bad road.</p><p>Your task is — for every possible <span class="tex-span"><i>x</i></span> determine the number of ways of improving the quality of some roads in order to meet the citizens' condition. As those values can be rather large, you need to print each value modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of cities in the country. Next line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i> - 1</span>) — the description of the roads in the country. Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that the country has a road connecting city <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and city <span class="tex-span"><i>i</i></span>. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the sought number of ways to improve the quality of the roads modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>), if the capital of the country is at city number <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of cities in the country. Next line contains <span class="tex-span"><i>n</i> - 1</span> positive integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, <i>p</i><sub class="lower-index">4</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>i</i> - 1</span>) — the description of the roads in the country. Number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that the country has a road connecting city <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and city <span class="tex-span"><i>i</i></span>. </p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the sought number of ways to improve the quality of the roads modulo <span class="tex-span">1 000 000 007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>), if the capital of the country is at city number <span class="tex-span"><i>i</i></span>.</p>





```input1
3
1 1

```




```input2
5
1 2 3 4

```




```output1
4 3 3
```




```output2
5 8 9 8 5
```


