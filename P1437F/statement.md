## Description

<div><p>$n$ fishermen have just returned from a fishing vacation. The $i$-th fisherman has caught a fish of weight $a_i$.</p><p>Fishermen are going to show off the fish they caught to each other. To do so, they firstly choose an order in which they show their fish (each fisherman shows his fish exactly once, so, formally, the order of showing fish is a permutation of integers from $1$ to $n$). Then they show the fish they caught according to the chosen order. When a fisherman shows his fish, he might either become happy, become sad, or stay content.</p><p>Suppose a fisherman shows a fish of weight $x$, and the maximum weight of a previously shown fish is $y$ ($y = 0$ if that fisherman is the first to show his fish). Then:</p><ul> <li> if $x \ge 2y$, the fisherman becomes happy; </li><li> if $2x \le y$, the fisherman becomes sad; </li><li> if none of these two conditions is met, the fisherman stays content. </li></ul><p>Let's call an order in which the fishermen show their fish <span class="tex-font-style-it">emotional</span> if, after all fishermen show their fish according to this order, each fisherman becomes either happy or sad. Calculate the number of <span class="tex-font-style-it">emotional</span> orders modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($2 \le n \le 5000$).</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^9$).</p></div><div class="output-specification"><p>Print one integer — the number of <span class="tex-font-style-it">emotional</span> orders, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($2 \le n \le 5000$).</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^9$).</p>

## Output

<p>Print one integer — the number of <span class="tex-font-style-it">emotional</span> orders, taken modulo $998244353$.</p>





```input1
4
1 1 4 9
```




```input2
4
4 3 2 1
```




```input3
3
4 2 1
```




```input4
8
42 1337 13 37 420 666 616 97
```




```output1
20
```




```output2
0
```




```output3
6
```




```output4
19200
```


