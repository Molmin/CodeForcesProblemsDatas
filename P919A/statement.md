## Description

<div><p>We often go to supermarkets to buy some fruits or vegetables, and on the tag there prints the price for a kilo. But in some supermarkets, when asked how much the items are, the clerk will say that $a$ <span class="tex-font-style-tt">yuan</span> for $b$ kilos (You don't need to care about what <span class="tex-font-style-tt">"yuan"</span> is), the same as $a/b$ <span class="tex-font-style-tt">yuan</span> for a kilo.</p><p>Now imagine you'd like to buy $m$ kilos of apples. You've asked $n$ supermarkets and got the prices. Find the minimum cost for those apples.</p><p>You can assume that there are enough apples in all supermarkets.</p></div><div class="input-specification"><p>The first line contains two positive integers $n$ and $m$ ($1 \leq n \leq 5\,000$, $1 \leq m \leq 100$), denoting that there are $n$ supermarkets and you want to buy $m$ kilos of apples.</p><p>The following $n$ lines describe the information of the supermarkets. Each line contains two positive integers $a, b$ ($1 \leq a, b \leq 100$), denoting that in this supermarket, you are supposed to pay $a$ <span class="tex-font-style-tt">yuan</span> for $b$ kilos of apples.</p></div><div class="output-specification"><p>The only line, denoting the minimum cost for $m$ kilos of apples. Please make sure that the absolute or relative error between your answer and the correct answer won't exceed $10^{-6}$.</p><p>Formally, let your answer be $x$, and the jury's answer be $y$. Your answer is considered correct if $\frac{|x - y|}{\max{(1, |y|)}} \le 10^{-6}$.</p></div>

## Input

<p>The first line contains two positive integers $n$ and $m$ ($1 \leq n \leq 5\,000$, $1 \leq m \leq 100$), denoting that there are $n$ supermarkets and you want to buy $m$ kilos of apples.</p><p>The following $n$ lines describe the information of the supermarkets. Each line contains two positive integers $a, b$ ($1 \leq a, b \leq 100$), denoting that in this supermarket, you are supposed to pay $a$ <span class="tex-font-style-tt">yuan</span> for $b$ kilos of apples.</p>

## Output

<p>The only line, denoting the minimum cost for $m$ kilos of apples. Please make sure that the absolute or relative error between your answer and the correct answer won't exceed $10^{-6}$.</p><p>Formally, let your answer be $x$, and the jury's answer be $y$. Your answer is considered correct if $\frac{|x - y|}{\max{(1, |y|)}} \le 10^{-6}$.</p>





```input1
3 5
1 2
3 4
1 3

```




```input2
2 1
99 100
98 99

```




```output1
1.66666667

```




```output2
0.98989899

```



## Note

<p>In the first sample, you are supposed to buy $5$ kilos of apples in supermarket $3$. The cost is $5/3$ <span class="tex-font-style-tt">yuan</span>.</p><p>In the second sample, you are supposed to buy $1$ kilo of apples in supermarket $2$. The cost is $98/99$ <span class="tex-font-style-tt">yuan</span>.</p>
