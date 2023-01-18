## Description

<div><p>You have $n$ coins, each of the same value of $1$.</p><p>Distribute them into packets such that any amount $x$ ($1 \leq x \leq n$) can be formed using some (possibly one or all) number of these packets.</p><p>Each packet may only be used entirely or not used at all. No packet may be used more than once in the formation of the single $x$, however it may be reused for the formation of other $x$'s.</p><p>Find the minimum number of packets in such a distribution.</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($1 \leq n \leq 10^9$)&nbsp;— the number of coins you have.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum possible number of packets, satisfying the condition above.</p></div>

## Input

<p>The only line contains a single integer $n$ ($1 \leq n \leq 10^9$)&nbsp;— the number of coins you have.</p>

## Output

<p>Output a single integer&nbsp;— the minimum possible number of packets, satisfying the condition above.</p>





```input1
6

```




```input2
2

```




```output1
3
```




```output2
2
```



## Note

<p>In the first example, three packets with $1$, $2$ and $3$ coins can be made to get any amount $x$ ($1\leq x\leq 6$).</p><ul> <li> To get $1$ use the packet with $1$ coin. </li><li> To get $2$ use the packet with $2$ coins. </li><li> To get $3$ use the packet with $3$ coins. </li><li> To get $4$ use packets with $1$ and $3$ coins. </li><li> To get $5$ use packets with $2$ and $3$ coins </li><li> To get $6$ use all packets. </li></ul><p>In the second example, two packets with $1$ and $1$ coins can be made to get any amount $x$ ($1\leq x\leq 2$).</p>
