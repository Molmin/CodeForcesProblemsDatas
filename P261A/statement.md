## Description

<div><p>Maxim always goes to the supermarket on Sundays. Today the supermarket has a special offer of discount systems.</p><p>There are <span class="tex-span"><i>m</i></span> types of discounts. We assume that the discounts are indexed from 1 to <span class="tex-span"><i>m</i></span>. To use the discount number <span class="tex-span"><i>i</i></span>, the customer takes a special basket, where he puts exactly <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> items he buys. Under the terms of the discount system, in addition to the items in the cart the customer can receive at most two items from the supermarket for free. The number of the "free items" (0, 1 or 2) to give is selected by the customer. The only condition imposed on the selected "free items" is as follows: each of them mustn't be more expensive than the cheapest item out of the <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> items in the cart.</p><p>Maxim now needs to buy <span class="tex-span"><i>n</i></span> items in the shop. Count the minimum sum of money that Maxim needs to buy them, if he use the discount system optimally well.</p><p>Please assume that the supermarket has enough carts for any actions. Maxim can use the same discount multiple times. Of course, Maxim can buy items without any discounts.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of discount types. The second line contains <span class="tex-span"><i>m</i></span> integers: <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>The third line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of items Maxim needs. The fourth line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the items' prices.</p><p>The numbers in the lines are separated by single spaces.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of discount types. The second line contains <span class="tex-span"><i>m</i></span> integers: <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span>. </p><p>The third line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of items Maxim needs. The fourth line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the items' prices.</p><p>The numbers in the lines are separated by single spaces.</p>

## Output

<p>In a single line print a single integer — the answer to the problem.</p>





```input1
1
2
4
50 50 100 100

```




```input2
2
2 3
5
50 50 50 50 50

```




```input3
1
1
7
1 1 1 1 1 1 1

```




```output1
200

```




```output2
150

```




```output3
3

```



## Note

<p>In the first sample Maxim needs to buy two items that cost <span class="tex-span">100</span> and get a discount for two free items that cost <span class="tex-span">50</span>. In that case, Maxim is going to pay <span class="tex-span">200</span>.</p><p>In the second sample the best strategy for Maxim is to buy <span class="tex-span">3</span> items and get <span class="tex-span">2</span> items for free using the discount. In that case, Maxim is going to pay <span class="tex-span">150</span>.</p>
