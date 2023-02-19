## Description

<div><p>You got a job as a marketer in a pet shop, and your current task is to boost sales of cat food. One of the strategies is to sell cans of food in packs with discounts. </p><p>Suppose you decided to sell packs with $a$ cans in a pack with a discount and some customer wants to buy $x$ cans of cat food. Then he follows a greedy strategy: </p><ul> <li> he buys $\left\lfloor \frac{x}{a} \right\rfloor$ packs with a discount; </li><li> then he wants to buy the remaining $(x \bmod a)$ cans one by one. </li></ul><p><span class="tex-font-style-it">$\left\lfloor \frac{x}{a} \right\rfloor$ is $x$ divided by $a$ rounded down, $x \bmod a$ is the remainer of $x$ divided by $a$.</span></p><p>But customers are greedy in general, so if the customer wants to buy $(x \bmod a)$ cans one by one and it happens that $(x \bmod a) \ge \frac{a}{2}$ he decides to buy the whole pack of $a$ cans (instead of buying $(x \bmod a)$ cans). It makes you, as a marketer, happy since the customer bought more than he wanted initially.</p><p>You know that each of the customers that come to your shop can buy any number of cans from $l$ to $r$ inclusive. Can you choose such size of pack $a$ that each customer buys more cans than they wanted initially?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $l$ and $r$ ($1 \le l \le r \le 10^9$)&nbsp;— the range of the number of cans customers can buy.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if you can choose such size of pack $a$ that each customer buys more cans than they wanted initially. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You can print each character in any case.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first and only line of each test case contains two integers $l$ and $r$ ($1 \le l \le r \le 10^9$)&nbsp;— the range of the number of cans customers can buy.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if you can choose such size of pack $a$ that each customer buys more cans than they wanted initially. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p><p>You can print each character in any case.</p>





```input1
3
3 4
1 2
120 150
```




```output1
YES
NO
YES
```



## Note

<p>In the first test case, you can take, for example, $a = 5$ as the size of the pack. Then if a customer wants to buy $3$ cans, he'll buy $5$ instead ($3 \bmod 5 = 3$, $\frac{5}{2} = 2.5$). The one who wants $4$ cans will also buy $5$ cans.</p><p>In the second test case, there is no way to choose $a$.</p><p>In the third test case, you can take, for example, $a = 80$.</p>
