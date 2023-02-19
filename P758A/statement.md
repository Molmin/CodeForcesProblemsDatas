## Description

<div><p>In Berland it is the holiday of equality. In honor of the holiday the king decided to equalize the welfare of all citizens in Berland by the expense of the state treasury. </p><p>Totally in Berland there are <span class="tex-span"><i>n</i></span> citizens, the welfare of each of them is estimated as the integer in <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> burles (burle is the currency in Berland).</p><p>You are the royal treasurer, which needs to count the minimum charges of the kingdom on the king's present. The king can only give money, he hasn't a power to take away them. </p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of citizens in the kingdom.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the welfare of the <span class="tex-span"><i>i</i></span>-th citizen.</p></div><div class="output-specification"><p>In the only line print the integer <span class="tex-span"><i>S</i></span>&nbsp;— the minimum number of burles which are had to spend.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of citizens in the kingdom.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the welfare of the <span class="tex-span"><i>i</i></span>-th citizen.</p>

## Output

<p>In the only line print the integer <span class="tex-span"><i>S</i></span>&nbsp;— the minimum number of burles which are had to spend.</p>





```input1
5
0 1 2 3 4

```




```input2
5
1 1 0 1 1

```




```input3
3
1 3 1

```




```input4
1
12

```




```output1
10
```




```output2
1
```




```output3
4
```




```output4
0
```



## Note

<p>In the first example if we add to the first citizen <span class="tex-span">4</span> burles, to the second <span class="tex-span">3</span>, to the third <span class="tex-span">2</span> and to the fourth <span class="tex-span">1</span>, then the welfare of all citizens will equal <span class="tex-span">4</span>.</p><p>In the second example it is enough to give one burle to the third citizen. </p><p>In the third example it is necessary to give two burles to the first and the third citizens to make the welfare of citizens equal <span class="tex-span">3</span>.</p><p>In the fourth example it is possible to give nothing to everyone because all citizens have <span class="tex-span">12</span> burles.</p>
