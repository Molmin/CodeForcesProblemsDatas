## Description

<div><p>Lavrenty, a baker, is going to make several buns with stuffings and sell them.</p><p>Lavrenty has <span class="tex-span"><i>n</i></span> grams of dough as well as <span class="tex-span"><i>m</i></span> different stuffing types. The stuffing types are numerated from 1 to <span class="tex-span"><i>m</i></span>. Lavrenty knows that he has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> grams left of the <span class="tex-span"><i>i</i></span>-th stuffing. It takes exactly <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> grams of stuffing <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> grams of dough to cook a bun with the <span class="tex-span"><i>i</i></span>-th stuffing. Such bun can be sold for <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> tugriks.</p><p>Also he can make buns <span class="tex-font-style-it">without stuffings</span>. Each of such buns requires <span class="tex-span"><i>c</i><sub class="lower-index">0</sub></span> grams of dough and it can be sold for <span class="tex-span"><i>d</i><sub class="lower-index">0</sub></span> tugriks. So Lavrenty can cook any number of buns with different stuffings or without it unless he runs out of dough and the stuffings. Lavrenty throws away all excess material left after baking.</p><p>Find the maximum number of tugriks Lavrenty can earn.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index">0</sub>, <i>d</i><sub class="lower-index">0</sub> ≤ 100</span>). Each of the following <span class="tex-span"><i>m</i></span> lines contains <span class="tex-span">4</span> integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Print the only number — the maximum number of tugriks Lavrenty can earn.</p></div>

## Input

<p>The first line contains <span class="tex-span">4</span> integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index">0</sub>, <i>d</i><sub class="lower-index">0</sub> ≤ 100</span>). Each of the following <span class="tex-span"><i>m</i></span> lines contains <span class="tex-span">4</span> integers. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>Print the only number — the maximum number of tugriks Lavrenty can earn.</p>





```input1
10 2 2 1
7 3 2 100
12 3 1 10

```




```input2
100 1 25 50
15 5 20 10

```




```output1
241
```




```output2
200
```



## Note

<p>To get the maximum number of tugriks in the first sample, you need to cook 2 buns with stuffing 1, 4 buns with stuffing 2 and a bun without any stuffing.</p><p>In the second sample Lavrenty should cook 4 buns without stuffings.</p>
