## Description

<div><p>Turbulent times are coming, so you decided to buy sugar in advance. There are $n$ shops around that sell sugar: the $i$-th shop sells one pack of sugar for $a_i$ coins, but only <span class="tex-font-style-bf">one pack to one customer</span> each day. So in order to buy several packs, you need to visit several shops.</p><p>Another problem is that prices are increasing each day: during the first day the cost is $a_i$, during the second day cost is $a_i + 1$, during the third day&nbsp;— $a_i + 2$ and so on for each shop $i$.</p><p>On the contrary, your everyday budget is only $x$ coins. In other words, each day you go and buy as many packs as possible with total cost not exceeding $x$. Note that if you don't spend some amount of coins during a day, you can't use these coins during the next days.</p><p>Eventually, the cost for each pack will exceed $x$, and you won't be able to buy even a single pack. So, how many packs will you be able to buy till that moment in total?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \le n \le 2 \cdot 10^5$; $1 \le x \le 10^9$)&nbsp;— the number of shops and your everyday budget.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the initial cost of one pack in each shop.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the total number of packs you will be able to buy until prices exceed your everyday budget.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains two integers $n$ and $x$ ($1 \le n \le 2 \cdot 10^5$; $1 \le x \le 10^9$)&nbsp;— the number of shops and your everyday budget.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the initial cost of one pack in each shop.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer&nbsp;— the total number of packs you will be able to buy until prices exceed your everyday budget.</p>





```input1
4
3 7
2 1 2
5 9
10 20 30 40 50
1 1
1
2 1000
1 1
```




```output1
11
0
1
1500
```



## Note

<p>In the first test case, </p><ul> <li> Day 1: prices are $[2, 1, 2]$. You can buy all $3$ packs, since $2 + 1 + 2 \le 7$. </li><li> Day 2: prices are $[3, 2, 3]$. You can't buy all $3$ packs, since $3 + 2 + 3 &gt; 7$, so you buy only $2$ packs. </li><li> Day 3: prices are $[4, 3, 4]$. You can buy $2$ packs with prices $4$ and $3$. </li><li> Day 4: prices are $[5, 4, 5]$. You can't buy $2$ packs anymore, so you buy only $1$ pack. </li><li> Day 5: prices are $[6, 5, 6]$. You can buy $1$ pack. </li><li> Day 6: prices are $[7, 6, 7]$. You can buy $1$ pack. </li><li> Day 7: prices are $[8, 7, 8]$. You still can buy $1$ pack of cost $7$. </li><li> Day 8: prices are $[9, 8, 9]$. Prices are too high, so you can't buy anything. </li></ul> In total, you bought $3 + 2 + 2 + 1 + 1 + 1 + 1 = 11$ packs.<p>In the second test case, prices are too high even at the first day, so you can't buy anything.</p><p>In the third test case, you can buy only one pack at day one.</p><p>In the fourth test case, you can buy $2$ packs first $500$ days. At day $501$ prices are $[501, 501]$, so you can buy only $1$ pack the next $500$ days. At day $1001$ prices are $[1001, 1001]$ so can't buy anymore. In total, you bought $500 \cdot 2 + 500 \cdot 1 = 1500$ packs.</p>
