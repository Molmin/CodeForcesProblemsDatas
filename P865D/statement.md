## Description

<div><p>You can perfectly predict the price of a certain stock for the next <span class="tex-span"><i>N</i></span> days. You would like to profit on this knowledge, but only want to transact one share of stock per day. That is, each day you will either buy one share, sell one share, or do nothing. Initially you own zero shares, and you cannot sell shares when you don't own any. At the end of the <span class="tex-span"><i>N</i></span> days you would like to again own zero shares, but want to have as much money as possible.</p></div><div class="input-specification"><p>Input begins with an integer <span class="tex-span"><i>N</i></span> <span class="tex-span">(2 ≤ <i>N</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>, the number of days.</p><p>Following this is a line with exactly <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>N</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. The price of one share of stock on the <span class="tex-span"><i>i</i></span>-th day is given by <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print the maximum amount of money you can end up with at the end of <span class="tex-span"><i>N</i></span> days.</p></div>

## Input

<p>Input begins with an integer <span class="tex-span"><i>N</i></span> <span class="tex-span">(2 ≤ <i>N</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>, the number of days.</p><p>Following this is a line with exactly <span class="tex-span"><i>N</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>N</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. The price of one share of stock on the <span class="tex-span"><i>i</i></span>-th day is given by <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print the maximum amount of money you can end up with at the end of <span class="tex-span"><i>N</i></span> days.</p>





```input1
9
10 5 4 7 9 12 6 2 10

```




```input2
20
3 1 4 1 5 9 2 6 5 3 5 8 9 7 9 3 2 3 8 4

```




```output1
20

```




```output2
41

```



## Note

<p>In the first example, buy a share at <span class="tex-span">5</span>, buy another at <span class="tex-span">4</span>, sell one at <span class="tex-span">9</span> and another at <span class="tex-span">12</span>. Then buy at <span class="tex-span">2</span> and sell at <span class="tex-span">10</span>. The total profit is <span class="tex-span"> - 5 - 4 + 9 + 12 - 2 + 10 = 20</span>.</p>
