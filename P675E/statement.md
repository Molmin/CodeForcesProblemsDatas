## Description

<div><p>Vasya commutes by train every day. There are <span class="tex-span"><i>n</i></span> train stations in the city, and at the <span class="tex-span"><i>i</i></span>-th station it's possible to buy only tickets to stations from <span class="tex-span"><i>i</i> + 1</span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> inclusive. No tickets are sold at the last station.</p><p>Let <span class="tex-span">ρ<sub class="lower-index"><i>i</i>, <i>j</i></sub></span> be the minimum number of tickets one needs to buy in order to get from stations <span class="tex-span"><i>i</i></span> to station <span class="tex-span"><i>j</i></span>. As Vasya is fond of different useless statistic he asks you to compute the sum of all values <span class="tex-span">ρ<sub class="lower-index"><i>i</i>, <i>j</i></sub></span> among all pairs <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of stations.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>i</i> + 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the <span class="tex-span"><i>i</i></span>-th of them means that at the <span class="tex-span"><i>i</i></span>-th station one may buy tickets to each station from <span class="tex-span"><i>i</i> + 1</span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> inclusive.</p></div><div class="output-specification"><p>Print the sum of <span class="tex-span">ρ<sub class="lower-index"><i>i</i>, <i>j</i></sub></span> among all pairs of <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of stations.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>i</i> + 1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the <span class="tex-span"><i>i</i></span>-th of them means that at the <span class="tex-span"><i>i</i></span>-th station one may buy tickets to each station from <span class="tex-span"><i>i</i> + 1</span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> inclusive.</p>

## Output

<p>Print the sum of <span class="tex-span">ρ<sub class="lower-index"><i>i</i>, <i>j</i></sub></span> among all pairs of <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>.</p>





```input1
4
4 4 4

```




```input2
5
2 3 5 5

```




```output1
6

```




```output2
17

```



## Note

<p>In the first sample it's possible to get from any station to any other (with greater index) using only one ticket. The total number of pairs is <span class="tex-span">6</span>, so the answer is also <span class="tex-span">6</span>.</p><p>Consider the second sample: </p><ul> <li> <span class="tex-span">ρ<sub class="lower-index">1, 2</sub> = 1</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">1, 3</sub> = 2</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">1, 4</sub> = 3</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">1, 5</sub> = 3</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">2, 3</sub> = 1</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">2, 4</sub> = 2</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">2, 5</sub> = 2</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">3, 4</sub> = 1</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">3, 5</sub> = 1</span> </li><li> <span class="tex-span">ρ<sub class="lower-index">4, 5</sub> = 1</span> </li></ul><p>Thus the answer equals <span class="tex-span">1 + 2 + 3 + 3 + 1 + 2 + 2 + 1 + 1 + 1 = 17</span>.</p>
