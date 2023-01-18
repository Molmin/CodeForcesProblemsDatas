## Description

<div><p>In this task you need to process a set of stock exchange orders and use them to create <span class="tex-font-style-it">order book</span>.</p><p>An <span class="tex-font-style-it">order</span> is an instruction of some participant to buy or sell stocks on stock exchange. The order number <span class="tex-span"><i>i</i></span> has price <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, direction <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> — buy or sell, and integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. This means that the participant is ready to buy or sell <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> stocks at price <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> for one stock. A value <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> is also known as a <span class="tex-font-style-it">volume</span> of an order.</p><p>All orders with the same price <span class="tex-span"><i>p</i></span> and direction <span class="tex-span"><i>d</i></span> are merged into one <span class="tex-font-style-it">aggregated</span> order with price <span class="tex-span"><i>p</i></span> and direction <span class="tex-span"><i>d</i></span>. The volume of such order is a sum of volumes of the initial orders.</p><p>An order book is a list of aggregated orders, the first part of which contains sell orders sorted by price in descending order, the second contains buy orders also sorted by price in descending order.</p><p>An order book of depth <span class="tex-span"><i>s</i></span> contains <span class="tex-span"><i>s</i></span> best aggregated orders for each direction. A buy order is better if it has higher price and a sell order is better if it has lower price. If there are less than <span class="tex-span"><i>s</i></span> aggregated orders for some direction then all of them will be in the final order book.</p><p>You are given <span class="tex-span"><i>n</i></span> stock exhange orders. Your task is to print order book of depth <span class="tex-span"><i>s</i></span> for these orders.</p></div><div class="input-specification"><p>The input starts with two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>s</i> ≤ 50</span>), the number of orders and the book depth.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains a letter <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (either '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">S</span>'), an integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) and an integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — direction, price and volume respectively. The letter '<span class="tex-font-style-tt">B</span>' means buy, '<span class="tex-font-style-tt">S</span>' means sell. The price of any sell order is higher than the price of any buy order.</p></div><div class="output-specification"><p>Print no more than <span class="tex-span">2<i>s</i></span> lines with aggregated orders from order book of depth <span class="tex-span"><i>s</i></span>. The output format for orders should be the same as in input.</p></div>

## Input

<p>The input starts with two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>s</i> ≤ 50</span>), the number of orders and the book depth.</p><p>Next <span class="tex-span"><i>n</i></span> lines contains a letter <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (either '<span class="tex-font-style-tt">B</span>' or '<span class="tex-font-style-tt">S</span>'), an integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) and an integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — direction, price and volume respectively. The letter '<span class="tex-font-style-tt">B</span>' means buy, '<span class="tex-font-style-tt">S</span>' means sell. The price of any sell order is higher than the price of any buy order.</p>

## Output

<p>Print no more than <span class="tex-span">2<i>s</i></span> lines with aggregated orders from order book of depth <span class="tex-span"><i>s</i></span>. The output format for orders should be the same as in input.</p>





```input1
6 2
B 10 3
S 50 2
S 40 1
S 50 6
B 20 4
B 25 10

```




```output1
S 50 8
S 40 1
B 25 10
B 20 4

```



## Note

<p>Denote <span class="tex-font-style-it">(x, y)</span> an order with price <span class="tex-span"><i>x</i></span> and volume <span class="tex-span"><i>y</i></span>. There are 3 aggregated buy orders (10, 3), (20, 4), (25, 10) and two sell orders (50, 8), (40, 1) in the sample.</p><p>You need to print no more than two best orders for each direction, so you shouldn't print the order (10 3) having the worst price among buy orders.</p>
