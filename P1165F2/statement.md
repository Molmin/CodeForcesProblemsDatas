## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is constraints</span>.</p><p>Ivan plays a computer game that contains some microtransactions to make characters look cooler. Since Ivan wants his character to be really cool, he wants to use some of these microtransactions — and he won't start playing until he gets all of them.</p><p>Each day (during the <span class="tex-font-style-bf">morning</span>) Ivan earns exactly one burle.</p><p>There are $n$ types of microtransactions in the game. Each microtransaction costs $2$ burles usually and $1$ burle if it is on sale. Ivan has to order exactly $k_i$ microtransactions of the $i$-th type (he orders microtransactions during the <span class="tex-font-style-bf">evening</span>).</p><p>Ivan can order <span class="tex-font-style-bf">any</span> (possibly zero) number of microtransactions of <span class="tex-font-style-bf">any</span> types during any day (of course, <span class="tex-font-style-bf">if he has enough money to do it</span>). If the microtransaction he wants to order is on sale then he can buy it for $1$ burle and otherwise he can buy it for $2$ burles.</p><p>There are also $m$ special offers in the game shop. The $j$-th offer $(d_j, t_j)$ means that microtransactions of the $t_j$-th type are on sale during the $d_j$-th day.</p><p>Ivan wants to order all microtransactions as soon as possible. Your task is to calculate the minimum day when he can buy all microtransactions he want and actually start playing.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the number of types of microtransactions and the number of special offers in the game shop.</p><p>The second line of the input contains $n$ integers $k_1, k_2, \dots, k_n$ ($0 \le k_i \le 2 \cdot 10^5$), where $k_i$ is the number of copies of microtransaction of the $i$-th type Ivan has to order. It is guaranteed that <span class="tex-font-style-bf">sum of all $k_i$ is not less than $1$ and not greater than $2 \cdot 10^5$</span>.</p><p>The next $m$ lines contain special offers. The $j$-th of these lines contains the $j$-th special offer. It is given as a pair of integers $(d_j, t_j)$ ($1 \le d_j \le 2 \cdot 10^5, 1 \le t_j \le n$) and means that microtransactions of the $t_j$-th type are on sale during the $d_j$-th day.</p></div><div class="output-specification"><p>Print one integer — the minimum day when Ivan can order all microtransactions he wants and actually start playing.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) — the number of types of microtransactions and the number of special offers in the game shop.</p><p>The second line of the input contains $n$ integers $k_1, k_2, \dots, k_n$ ($0 \le k_i \le 2 \cdot 10^5$), where $k_i$ is the number of copies of microtransaction of the $i$-th type Ivan has to order. It is guaranteed that <span class="tex-font-style-bf">sum of all $k_i$ is not less than $1$ and not greater than $2 \cdot 10^5$</span>.</p><p>The next $m$ lines contain special offers. The $j$-th of these lines contains the $j$-th special offer. It is given as a pair of integers $(d_j, t_j)$ ($1 \le d_j \le 2 \cdot 10^5, 1 \le t_j \le n$) and means that microtransactions of the $t_j$-th type are on sale during the $d_j$-th day.</p>

## Output

<p>Print one integer — the minimum day when Ivan can order all microtransactions he wants and actually start playing.</p>





```input1
5 6
1 2 0 2 0
2 4
3 3
1 5
1 2
1 5
2 3
```




```input2
5 3
4 2 1 3 2
3 5
4 2
2 5
```




```output1
8
```




```output2
20
```


