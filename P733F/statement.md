## Description

<div><p>In one kingdom there are <span class="tex-span"><i>n</i></span> cities and <span class="tex-span"><i>m</i></span> two-way roads. Each road connects a pair of cities, and for each road we know the level of drivers dissatisfaction&nbsp;— the value <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>For each road we know the value <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— how many lamziks we should spend to reduce the level of dissatisfaction with this road by one. Thus, to reduce the dissatisfaction with the <span class="tex-span"><i>i</i></span>-th road by <span class="tex-span"><i>k</i></span>, we should spend <span class="tex-span"><i>k</i>·<i>c</i><sub class="lower-index"><i>i</i></sub></span> lamziks. And <span class="tex-font-style-bf">it is allowed for the dissatisfaction to become zero or even negative</span>.</p><p>In accordance with the king's order, we need to choose <span class="tex-span"><i>n</i> - 1</span> roads and make them the <span class="tex-font-style-it">main roads</span>. An important condition must hold: it should be possible to travel from any city to any other by the <span class="tex-font-style-it">main roads</span>.</p><p>The road ministry has a budget of <span class="tex-span"><i>S</i></span> lamziks for the reform. The ministry is going to spend this budget for repair of some roads (to reduce the dissatisfaction with them), and then to choose the <span class="tex-span"><i>n</i> - 1</span> <span class="tex-font-style-it">main roads</span>.</p><p>Help to spend the budget in such a way and then to choose the main roads so that the total dissatisfaction with the <span class="tex-font-style-it">main roads</span> will be as small as possible. The dissatisfaction with some roads can become negative. It is not necessary to spend whole budget <span class="tex-span"><i>S</i></span>.</p><p>It is guaranteed that it is possible to travel from any city to any other using existing roads. Each road in the kingdom is a two-way road.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cities and the number of roads in the kingdom, respectively.</p><p>The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the drivers dissatisfaction with the <span class="tex-span"><i>i</i></span>-th road.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the cost (in lamziks) of reducing the dissatisfaction with the <span class="tex-span"><i>i</i></span>-th road by one.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the description of the roads. The <span class="tex-span"><i>i</i></span>-th of this lines contain a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) which mean that the <span class="tex-span"><i>i</i></span>-th road connects cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. All roads are two-way oriented so it is possible to move by the <span class="tex-span"><i>i</i></span>-th road from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and vice versa. It is allowed that a pair of cities is connected by more than one road. </p><p>The last line contains one integer <span class="tex-span"><i>S</i></span> (<span class="tex-span">0 ≤ <i>S</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of lamziks which we can spend for reforms. </p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>K</i></span>&nbsp;— the minimum possible total dissatisfaction with <span class="tex-font-style-it">main roads</span>.</p><p>In each of the next <span class="tex-span"><i>n</i> - 1</span> lines print two integers <span class="tex-span"><i>x</i>, <i>v</i><sub class="lower-index"><i>x</i></sub></span>, which mean that the road <span class="tex-span"><i>x</i></span> is among main roads and the road <span class="tex-span"><i>x</i></span>, after the reform, has the level of dissatisfaction <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub></span>.</p><p>Consider that roads are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order as they are given in the input data. The edges can be printed in arbitrary order. If there are several answers, print any of them. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> - 1 ≤ <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cities and the number of roads in the kingdom, respectively.</p><p>The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is the drivers dissatisfaction with the <span class="tex-span"><i>i</i></span>-th road.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the cost (in lamziks) of reducing the dissatisfaction with the <span class="tex-span"><i>i</i></span>-th road by one.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the description of the roads. The <span class="tex-span"><i>i</i></span>-th of this lines contain a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) which mean that the <span class="tex-span"><i>i</i></span>-th road connects cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. All roads are two-way oriented so it is possible to move by the <span class="tex-span"><i>i</i></span>-th road from <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and vice versa. It is allowed that a pair of cities is connected by more than one road. </p><p>The last line contains one integer <span class="tex-span"><i>S</i></span> (<span class="tex-span">0 ≤ <i>S</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of lamziks which we can spend for reforms. </p>

## Output

<p>In the first line print <span class="tex-span"><i>K</i></span>&nbsp;— the minimum possible total dissatisfaction with <span class="tex-font-style-it">main roads</span>.</p><p>In each of the next <span class="tex-span"><i>n</i> - 1</span> lines print two integers <span class="tex-span"><i>x</i>, <i>v</i><sub class="lower-index"><i>x</i></sub></span>, which mean that the road <span class="tex-span"><i>x</i></span> is among main roads and the road <span class="tex-span"><i>x</i></span>, after the reform, has the level of dissatisfaction <span class="tex-span"><i>v</i><sub class="lower-index"><i>x</i></sub></span>.</p><p>Consider that roads are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order as they are given in the input data. The edges can be printed in arbitrary order. If there are several answers, print any of them. </p>





```input1
6 9
1 3 1 1 3 1 2 2 2
4 1 4 2 2 5 3 1 6
1 2
1 3
2 3
2 4
2 5
3 5
3 6
4 5
5 6
7

```




```input2
3 3
9 5 1
7 7 2
2 1
3 1
3 2
2

```




```output1
0
1 1
3 1
6 1
7 2
8 -5

```




```output2
5
3 0
2 5

```


