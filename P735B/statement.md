## Description

<div><p>Local authorities have heard a lot about combinatorial abilities of Ostap Bender so they decided to ask his help in the question of urbanization. There are <span class="tex-span"><i>n</i></span> people who plan to move to the cities. The wealth of the <span class="tex-span"><i>i</i></span> of them is equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Authorities plan to build two cities, first for <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> people and second for <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> people. Of course, each of <span class="tex-span"><i>n</i></span> candidates can settle in only one of the cities. Thus, first some subset of candidates of size <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> settle in the first city and then some subset of size <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> is chosen among the remaining candidates and the move to the second city. All other candidates receive an official refuse and go back home.</p><p>To make the statistic of local region look better in the eyes of their bosses, local authorities decided to pick subsets of candidates in such a way that <span class="tex-font-style-bf">the sum of arithmetic mean</span> of wealth of people in each of the cities is as large as possible. Arithmetic mean of wealth in one city is the sum of wealth <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> among all its residents divided by the number of them (<span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> or <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> depending on the city). The division should be done in real numbers without any rounding.</p><p>Please, help authorities find the optimal way to pick residents for two cities.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub> ≤ 100 000</span>, <span class="tex-span"><i>n</i><sub class="lower-index">1</sub> + <i>n</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>)&nbsp;— the number of candidates who want to move to the cities, the planned number of residents of the first city and the planned number of residents of the second city.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the wealth of the <span class="tex-span"><i>i</i></span>-th candidate.</p></div><div class="output-specification"><p>Print one real value&nbsp;— the maximum possible sum of arithmetic means of wealth of cities' residents. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://89PVECnm.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>n</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>n</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>n</i><sub class="lower-index">1</sub>, <i>n</i><sub class="lower-index">2</sub> ≤ 100 000</span>, <span class="tex-span"><i>n</i><sub class="lower-index">1</sub> + <i>n</i><sub class="lower-index">2</sub> ≤ <i>n</i></span>)&nbsp;— the number of candidates who want to move to the cities, the planned number of residents of the first city and the planned number of residents of the second city.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the wealth of the <span class="tex-span"><i>i</i></span>-th candidate.</p>

## Output

<p>Print one real value&nbsp;— the maximum possible sum of arithmetic means of wealth of cities' residents. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://89PVECnm.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
2 1 1
1 5

```




```input2
4 2 1
1 4 2 3

```




```output1
6.00000000

```




```output2
6.50000000

```



## Note

<p>In the first sample, one of the optimal solutions is to move candidate <span class="tex-span">1</span> to the first city and candidate <span class="tex-span">2</span> to the second.</p><p>In the second sample, the optimal solution is to pick candidates <span class="tex-span">3</span> and <span class="tex-span">4</span> for the first city, and candidate <span class="tex-span">2</span> for the second one. Thus we obtain <span class="tex-span">(<i>a</i><sub class="lower-index">3</sub> + <i>a</i><sub class="lower-index">4</sub>) / 2 + <i>a</i><sub class="lower-index">2</sub> = (3 + 2) / 2 + 4 = 6.5</span></p>
