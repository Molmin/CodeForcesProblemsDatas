## Description

<div><p>Vasya often uses public transport. The transport in the city is of two types: trolleys and buses. The city has <span class="tex-span"><i>n</i></span> buses and <span class="tex-span"><i>m</i></span> trolleys, the buses are numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the trolleys are numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>Public transport is not free. There are 4 types of tickets: </p><ol> <li> A ticket for one ride on some bus or trolley. It costs <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> burles; </li><li> A ticket for an unlimited number of rides on some bus or on some trolley. It costs <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> burles; </li><li> A ticket for an unlimited number of rides on all buses or all trolleys. It costs <span class="tex-span"><i>c</i><sub class="lower-index">3</sub></span> burles; </li><li> A ticket for an unlimited number of rides on all buses and trolleys. It costs <span class="tex-span"><i>c</i><sub class="lower-index">4</sub></span> burles. </li></ol><p>Vasya knows for sure the number of rides he is going to make and the transport he is going to use. He asked you for help to find the minimum sum of burles he will have to spend on the tickets.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub> ≤ 1000)</span> — the costs of the tickets.</p><p>The second line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span> — the number of buses and trolleys Vasya is going to use.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the number of times Vasya is going to use the bus number <span class="tex-span"><i>i</i></span>.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the number of times Vasya is going to use the trolley number <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print a single number — the minimum sum of burles Vasya will have to spend on the tickets.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">4</sub> ≤ 1000)</span> — the costs of the tickets.</p><p>The second line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span> — the number of buses and trolleys Vasya is going to use.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the number of times Vasya is going to use the bus number <span class="tex-span"><i>i</i></span>.</p><p>The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the number of times Vasya is going to use the trolley number <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print a single number — the minimum sum of burles Vasya will have to spend on the tickets.</p>





```input1
1 3 7 19
2 3
2 5
4 4 4

```




```input2
4 3 2 1
1 3
798
1 2 3

```




```input3
100 100 8 100
3 5
7 94 12
100 1 47 0 42

```




```output1
12

```




```output2
1

```




```output3
16

```



## Note

<p>In the first sample the profitable strategy is to buy two tickets of the first type (for the first bus), one ticket of the second type (for the second bus) and one ticket of the third type (for all trolleys). It totals to <span class="tex-span">(2·1) + 3 + 7 = 12</span> burles.</p><p>In the second sample the profitable strategy is to buy one ticket of the fourth type.</p><p>In the third sample the profitable strategy is to buy two tickets of the third type: for all buses and for all trolleys.</p>
