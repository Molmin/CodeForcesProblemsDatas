## Description

<div><p>The New Year celebrations in Berland last <span class="tex-span"><i>n</i></span> days. Only this year the winter is snowless, that’s why the winter celebrations’ organizers should buy artificial snow. There are <span class="tex-span"><i>m</i></span> snow selling companies in Berland. Every day the <span class="tex-span"><i>i</i></span>-th company produces <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> cubic meters of snow. Next day the snow thaws and the company has to produce <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> cubic meters of snow again. During the celebration new year discounts are on, that’s why the snow cost decreases every day. It is known that on the first day the total cost of all the snow produced by the <span class="tex-span"><i>i</i></span>-th company is equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> bourles. Every day this total cost decreases by <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bourles, i.e. on the second day it is equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i></sub></span>,and on the third day — to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> - 2<i>a</i><sub class="lower-index"><i>i</i></sub></span>, and so on. It is known that for one company the cost of the snow produced by it does not get negative or equal to zero. You have to organize the snow purchase so as to buy every day exactly <span class="tex-span"><i>W</i></span> snow cubic meters. At that it is not necessary to buy from any company all the snow produced by it. If you buy <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> cubic meters of snow (<span class="tex-span">0 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i><sub class="lower-index"><i>i</i></sub></span>, the number <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> is not necessarily integer!) from the <span class="tex-span"><i>i</i></span>-th company at one of the days when the cost of its snow is equal to <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, then its price will total to <img align="middle" class="tex-formula" src="file://Ig5606IL.png" style="max-width: 100.0%;max-height: 100.0%;"> bourles. During one day one can buy the snow from several companies. In different days one can buy the snow from different companies. It is required to make the purchases so as to spend as little money as possible. It is guaranteed that the snow produced by the companies will be enough.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>W</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 500000</span>, <span class="tex-span">1 ≤ <i>W</i> ≤ 10<sup class="upper-index">9</sup></span>) which represent the number of days, the number of companies and the amount of snow that needs to be purchased on every one of the <span class="tex-span"><i>n</i></span> days. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. All the numbers are strictly positive and do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. For all the <span class="tex-span"><i>i</i></span> the inequation <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> - (<i>n</i> - 1)<i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> holds true. </p></div><div class="output-specification"><p>Print a single number — the answer to the given problem. Print the answer in the format with the decimal point (even if the answer is integer, it must contain the decimal point), without "e" and without leading zeroes. The answer should differ with the right one by no more than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>W</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 500000</span>, <span class="tex-span">1 ≤ <i>W</i> ≤ 10<sup class="upper-index">9</sup></span>) which represent the number of days, the number of companies and the amount of snow that needs to be purchased on every one of the <span class="tex-span"><i>n</i></span> days. The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The fourth line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. All the numbers are strictly positive and do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. For all the <span class="tex-span"><i>i</i></span> the inequation <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> - (<i>n</i> - 1)<i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span> holds true. </p>

## Output

<p>Print a single number — the answer to the given problem. Print the answer in the format with the decimal point (even if the answer is integer, it must contain the decimal point), without "e" and without leading zeroes. The answer should differ with the right one by no more than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
2 3 10
4 4 4
5 5 8
1 2 5

```




```input2
100 2 1000000000
999999998 999999999
1000000000 1000000000
1 1

```




```output1
22.000000000000000

```




```output2
99999995149.999995249999991

```


