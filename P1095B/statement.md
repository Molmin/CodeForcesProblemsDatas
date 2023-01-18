## Description

<div><p>You are given an array $a$ consisting of $n$ integer numbers.</p><p>Let <span class="tex-font-style-it">instability</span> of the array be the following value: $\max\limits_{i = 1}^{n} a_i - \min\limits_{i = 1}^{n} a_i$.</p><p>You have to remove <span class="tex-font-style-bf">exactly one</span> element from this array to minimize <span class="tex-font-style-it">instability</span> of the resulting $(n-1)$-elements array. Your task is to calculate the minimum possible <span class="tex-font-style-it">instability</span>.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($2 \le n \le 10^5$) — the number of elements in the array $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$) — elements of the array $a$.</p></div><div class="output-specification"><p>Print one integer — the minimum possible <span class="tex-font-style-it">instability</span> of the array if you have to remove <span class="tex-font-style-bf">exactly one</span> element from the array $a$.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($2 \le n \le 10^5$) — the number of elements in the array $a$.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$) — elements of the array $a$.</p>

## Output

<p>Print one integer — the minimum possible <span class="tex-font-style-it">instability</span> of the array if you have to remove <span class="tex-font-style-bf">exactly one</span> element from the array $a$.</p>





```input1
4
1 3 3 7
```




```input2
2
1 100000
```




```output1
2
```




```output2
0
```



## Note

<p>In the first example you can remove $7$ then <span class="tex-font-style-it">instability</span> of the remaining array will be $3 - 1 = 2$.</p><p>In the second example you can remove either $1$ or $100000$ then <span class="tex-font-style-it">instability</span> of the remaining array will be $100000 - 100000 = 0$ and $1 - 1 = 0$ correspondingly.</p>
