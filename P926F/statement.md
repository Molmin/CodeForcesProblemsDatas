## Description

<div><p>A sum of <span class="tex-span"><i>p</i></span> rubles is charged from Arkady's mobile phone account every day in the morning. Among the following <span class="tex-span"><i>m</i></span> days, there are <span class="tex-span"><i>n</i></span> days when Arkady will top up the account: in the day <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> he will deposit <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> rubles on his mobile phone account. Arkady will always top up the account before the daily payment will be done. There will be no other payments nor tops up in the following <span class="tex-span"><i>m</i></span> days.</p><p>Determine the number of days starting from the <span class="tex-span">1</span>-st to the <span class="tex-span"><i>m</i></span>-th such that the account will have a negative amount on it after the daily payment (i.&nbsp;e. in evening). Initially the account's balance is zero rubles.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>n</i> ≤ <i>m</i></span>) — the number of days Arkady will top up the account, the amount of the daily payment, and the number of days you should check.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the index of the day when Arkady will make the <span class="tex-span"><i>i</i></span>-th top up, and the amount he will deposit on this day. It is guaranteed that the indices of the days are distinct and are given in increasing order, i.&nbsp;e. <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &gt; <i>d</i><sub class="lower-index"><i>i</i> - 1</sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Print the number of days from the <span class="tex-span">1</span>-st to the <span class="tex-span"><i>m</i></span>-th such that the account will have a negative amount on it after the daily payment.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>n</i> ≤ <i>m</i></span>) — the number of days Arkady will top up the account, the amount of the daily payment, and the number of days you should check.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the index of the day when Arkady will make the <span class="tex-span"><i>i</i></span>-th top up, and the amount he will deposit on this day. It is guaranteed that the indices of the days are distinct and are given in increasing order, i.&nbsp;e. <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &gt; <i>d</i><sub class="lower-index"><i>i</i> - 1</sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Print the number of days from the <span class="tex-span">1</span>-st to the <span class="tex-span"><i>m</i></span>-th such that the account will have a negative amount on it after the daily payment.</p>





```input1
3 6 7
2 13
4 20
7 9

```




```input2
5 4 100
10 70
15 76
21 12
30 100
67 85

```




```output1
3

```




```output2
26

```



## Note

<p>In the first example the balance will change as following (remember, initially the balance is zero):</p><ol> <li> in the first day <span class="tex-span">6</span> rubles will be charged, the balance in the evening will be equal to <span class="tex-span"> - 6</span>; </li><li> in the second day Arkady will deposit <span class="tex-span">13</span> rubles, then <span class="tex-span">6</span> rubles will be charged, the balance in the evening will be equal to <span class="tex-span">1</span>; </li><li> in the third day <span class="tex-span">6</span> rubles will be charged, the balance in the evening will be equal to <span class="tex-span"> - 5</span>; </li><li> in the fourth day Arkady will deposit <span class="tex-span">20</span> rubles, then <span class="tex-span">6</span> rubles will be charged, the balance in the evening will be equal to <span class="tex-span">9</span>; </li><li> in the fifth day <span class="tex-span">6</span> rubles will be charged, the balance in the evening will be equal to <span class="tex-span">3</span>; </li><li> in the sixth day <span class="tex-span">6</span> rubles will be charged, the balance in the evening will be equal to <span class="tex-span"> - 3</span>; </li><li> in the seventh day Arkady will deposit <span class="tex-span">9</span> rubles, then <span class="tex-span">6</span> rubles will be charged, the balance in the evening will be equal to <span class="tex-span">0</span>. </li></ol><p>Thus, in the end of the first, third and sixth days the balance will be negative in the end of the day.</p>
