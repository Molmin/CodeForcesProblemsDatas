## Description

<div><p>Enough is enough. Too many times it happened that Vasya forgot to dispose of garbage and his apartment stank afterwards. Now he wants to create a garbage disposal plan and stick to it.</p><p>For each of next $n$ days Vasya knows $a_i$ — number of <span class="tex-font-style-it">units of garbage</span> he will produce on the $i$-th day. Each <span class="tex-font-style-it">unit of garbage</span> must be disposed of either on the day it was produced or on the next day. Vasya disposes of garbage by putting it inside a bag and dropping the bag into a garbage container. Each bag can contain up to $k$ <span class="tex-font-style-it">units of garbage</span>. It is allowed to compose and drop multiple bags into a garbage container in a single day.</p><p>Being economical, Vasya wants to use as few bags as possible. You are to compute the minimum number of bags Vasya needs to dispose of all of his garbage for the given $n$ days. No garbage should be left after the $n$-th day.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 2\cdot10^5, 1 \le k \le 10^9$) — number of days to consider and bag's capacity. The second line contains $n$ space separated integers $a_i$ ($0 \le a_i \le 10^9$) — the number of <span class="tex-font-style-it">units of garbage</span> produced on the $i$-th day.</p></div><div class="output-specification"><p>Output a single integer — the minimum number of bags Vasya needs to dispose of all garbage. Each <span class="tex-font-style-it">unit of garbage</span> should be disposed on the day it was produced or on the next day. No garbage can be left after the $n$-th day. In a day it is allowed to compose and drop multiple bags.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 2\cdot10^5, 1 \le k \le 10^9$) — number of days to consider and bag's capacity. The second line contains $n$ space separated integers $a_i$ ($0 \le a_i \le 10^9$) — the number of <span class="tex-font-style-it">units of garbage</span> produced on the $i$-th day.</p>

## Output

<p>Output a single integer — the minimum number of bags Vasya needs to dispose of all garbage. Each <span class="tex-font-style-it">unit of garbage</span> should be disposed on the day it was produced or on the next day. No garbage can be left after the $n$-th day. In a day it is allowed to compose and drop multiple bags.</p>





```input1
3 2
3 2 1

```




```input2
5 1
1000000000 1000000000 1000000000 1000000000 1000000000

```




```input3
3 2
1 0 1

```




```input4
4 4
2 8 4 1

```




```output1
3

```




```output2
5000000000

```




```output3
2

```




```output4
4

```


