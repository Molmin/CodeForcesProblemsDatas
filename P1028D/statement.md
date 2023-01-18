## Description

<div><p>Let's consider a simplified version of order book of some stock. The order book is a list of orders (offers) from people that want to buy or sell one unit of the stock, each order is described by <span class="tex-font-style-it">direction</span> (<span class="tex-font-style-tt">BUY</span> or <span class="tex-font-style-tt">SELL</span>) and price.</p><p>At every moment of time, every <span class="tex-font-style-tt">SELL</span> offer has higher price than every <span class="tex-font-style-tt">BUY</span> offer. </p><p><span class="tex-font-style-bf">In this problem no two ever existed orders will have the same price.</span></p><p>The lowest-price <span class="tex-font-style-tt">SELL</span> order and the highest-price <span class="tex-font-style-tt">BUY</span> order are called the <span class="tex-font-style-it">best offers</span>, marked with black frames on the picture below.</p><center> <img class="tex-graphics" src="file://mY11JdDB.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The presented order book says that someone wants to sell the product at price $12$ and it's the best <span class="tex-font-style-tt">SELL</span> offer because the other two have higher prices. The best <span class="tex-font-style-tt">BUY</span> offer has price $10$.</span> </center><p>There are two possible actions in this orderbook: </p><ol><li> Somebody adds a new order of some direction with some price.</li><li> Somebody accepts the best possible <span class="tex-font-style-tt">SELL</span> or <span class="tex-font-style-tt">BUY</span> offer (makes a deal). It's impossible to accept not the best <span class="tex-font-style-tt">SELL</span> or <span class="tex-font-style-tt">BUY</span> offer (to make a deal at worse price). After someone accepts the offer, it is removed from the orderbook forever.</li></ol><p>It is allowed to add new <span class="tex-font-style-tt">BUY</span> order only with prices less than the best <span class="tex-font-style-tt">SELL</span> offer (if you want to buy stock for higher price, then instead of adding an order you should accept the best <span class="tex-font-style-tt">SELL</span> offer). Similarly, one couldn't add a new <span class="tex-font-style-tt">SELL</span> order with price less or equal to the best <span class="tex-font-style-tt">BUY</span> offer. For example, you can't add a new offer "<span class="tex-font-style-tt">SELL</span> $20$" if there is already an offer "<span class="tex-font-style-tt">BUY</span> $20$" or "<span class="tex-font-style-tt">BUY</span> $25$"&nbsp;— in this case you just accept the best <span class="tex-font-style-tt">BUY</span> offer.</p><p>You have a damaged order book log (in the beginning the are no orders in book). Every action has one of the two types:</p><ol><li> "<span class="tex-font-style-tt">ADD</span> $p$" denotes adding a new order with price $p$ and unknown direction. The order must not contradict with orders still not removed from the order book. </li><li> "<span class="tex-font-style-tt">ACCEPT</span> $p$" denotes accepting an existing best offer with price $p$ and unknown direction.</li></ol><p>The directions of all actions are lost. Information from the log isn't always enough to determine these directions. Count the number of ways to correctly restore all <span class="tex-font-style-tt">ADD</span> action directions so that all the described conditions are satisfied at any moment. Since the answer could be large, output it modulo $10^9 + 7$. If it is impossible to correctly restore directions, then output $0$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 363\,304$) — the number of actions in the log.</p><p>Each of the next $n$ lines contains a string "<span class="tex-font-style-tt">ACCEPT</span>" or "<span class="tex-font-style-tt">ADD</span>" and an integer $p$ ($1 \le p \le 308\,983\,066$), describing an action type and price. </p><p>All <span class="tex-font-style-tt">ADD</span> actions have different prices. For <span class="tex-font-style-tt">ACCEPT</span> action it is guaranteed that the order with the same price has already been added but has not been accepted yet.</p></div><div class="output-specification"><p>Output the number of ways to restore directions of <span class="tex-font-style-tt">ADD</span> actions modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 363\,304$) — the number of actions in the log.</p><p>Each of the next $n$ lines contains a string "<span class="tex-font-style-tt">ACCEPT</span>" or "<span class="tex-font-style-tt">ADD</span>" and an integer $p$ ($1 \le p \le 308\,983\,066$), describing an action type and price. </p><p>All <span class="tex-font-style-tt">ADD</span> actions have different prices. For <span class="tex-font-style-tt">ACCEPT</span> action it is guaranteed that the order with the same price has already been added but has not been accepted yet.</p>

## Output

<p>Output the number of ways to restore directions of <span class="tex-font-style-tt">ADD</span> actions modulo $10^9 + 7$.</p>





```input1
6
ADD 1
ACCEPT 1
ADD 2
ACCEPT 2
ADD 3
ACCEPT 3

```




```input2
4
ADD 1
ADD 2
ADD 3
ACCEPT 2

```




```input3
7
ADD 1
ADD 2
ADD 3
ADD 4
ADD 5
ACCEPT 3
ACCEPT 5

```




```output1
8

```




```output2
2

```




```output3
0

```



## Note

<p>In the first example each of orders may be <span class="tex-font-style-tt">BUY</span> or <span class="tex-font-style-tt">SELL</span>.</p><p>In the second example the order with price $1$ has to be <span class="tex-font-style-tt">BUY</span> order, the order with the price $3$ has to be <span class="tex-font-style-tt">SELL</span> order.</p>
