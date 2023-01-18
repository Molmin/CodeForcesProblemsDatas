## Description

<div><p>There are $n$ people in this world, conveniently numbered $1$ through $n$. They are using burles to buy goods and services. Occasionally, a person might not have enough currency to buy what he wants or needs, so he borrows money from someone else, with the idea that he will repay the loan later with interest. Let $d(a,b)$ denote the debt of $a$ towards $b$, or $0$ if there is no such debt.</p><p>Sometimes, this becomes very complex, as the person lending money can run into financial troubles before his debtor is able to repay his debt, and finds himself in the need of borrowing money. </p><p>When this process runs for a long enough time, it might happen that there are so many debts that they can be consolidated. There are two ways this can be done:</p><ol> <li> Let $d(a,b) &gt; 0$ and $d(c,d) &gt; 0$ such that $a \neq c$ or $b \neq d$. We can decrease the $d(a,b)$ and $d(c,d)$ by&nbsp;$z$ and increase $d(c,b)$ and $d(a,d)$ by&nbsp;$z$, where $0 &lt; z \leq \min(d(a,b),d(c,d))$. </li><li> Let $d(a,a) &gt; 0$. We can set $d(a,a)$ to $0$. </li></ol><p>The total debt is defined as the sum of all debts:</p><p>$$\Sigma_d = \sum_{a,b} d(a,b)$$</p><p>Your goal is to use the above rules in any order any number of times, to make the total debt as small as possible. Note that you don't have to minimise the <span class="tex-font-style-bf">number</span> of non-zero debts, only the <span class="tex-font-style-bf">total debt</span>.</p></div><div class="input-specification"><p>The first line contains two space separated integers $n$&nbsp;($1 \leq n \leq 10^5$) and $m$&nbsp;($0 \leq m \leq 3\cdot 10^5$), representing the number of people and the number of debts, respectively.</p><p>$m$ lines follow, each of which contains three space separated integers $u_i$, $v_i$&nbsp;($1 \leq u_i, v_i \leq n, u_i \neq v_i$), $d_i$&nbsp;($1 \leq d_i \leq 10^9$), meaning that the person $u_i$ borrowed $d_i$ burles from person $v_i$.</p></div><div class="output-specification"><p>On the first line print an integer $m'$&nbsp;($0 \leq m' \leq 3\cdot 10^5$), representing the number of debts after the consolidation. It can be shown that an answer always exists with this additional constraint.</p><p>After that print $m'$ lines, $i$-th of which contains three space separated integers $u_i, v_i, d_i$, meaning that the person $u_i$ owes the person $v_i$ exactly $d_i$ burles. The output must satisfy $1 \leq u_i, v_i \leq n$, $u_i \neq v_i$ and $0 &lt; d_i \leq 10^{18}$.</p><p>For each pair $i \neq j$, it should hold that $u_i \neq u_j$ or $v_i \neq v_j$. In other words, each pair of people can be included at most once in the output.</p></div>

## Input

<p>The first line contains two space separated integers $n$&nbsp;($1 \leq n \leq 10^5$) and $m$&nbsp;($0 \leq m \leq 3\cdot 10^5$), representing the number of people and the number of debts, respectively.</p><p>$m$ lines follow, each of which contains three space separated integers $u_i$, $v_i$&nbsp;($1 \leq u_i, v_i \leq n, u_i \neq v_i$), $d_i$&nbsp;($1 \leq d_i \leq 10^9$), meaning that the person $u_i$ borrowed $d_i$ burles from person $v_i$.</p>

## Output

<p>On the first line print an integer $m'$&nbsp;($0 \leq m' \leq 3\cdot 10^5$), representing the number of debts after the consolidation. It can be shown that an answer always exists with this additional constraint.</p><p>After that print $m'$ lines, $i$-th of which contains three space separated integers $u_i, v_i, d_i$, meaning that the person $u_i$ owes the person $v_i$ exactly $d_i$ burles. The output must satisfy $1 \leq u_i, v_i \leq n$, $u_i \neq v_i$ and $0 &lt; d_i \leq 10^{18}$.</p><p>For each pair $i \neq j$, it should hold that $u_i \neq u_j$ or $v_i \neq v_j$. In other words, each pair of people can be included at most once in the output.</p>





```input1
3 2
1 2 10
2 3 5

```




```input2
3 3
1 2 10
2 3 15
3 1 10

```




```input3
4 2
1 2 12
3 4 8

```




```input4
3 4
2 3 1
2 3 2
2 3 4
2 3 8

```




```output1
2
1 2 5
1 3 5

```




```output2
1
2 3 5

```




```output3
2
1 2 12
3 4 8

```




```output4
1
2 3 15

```



## Note

<p>In the first example the optimal sequence of operations can be the following:</p><ol> <li> Perform an operation of the first type with $a = 1$, $b = 2$, $c = 2$, $d = 3$ and $z = 5$. The resulting debts are: $d(1, 2) = 5$, $d(2, 2) = 5$, $d(1, 3) = 5$, all other debts are $0$; </li><li> Perform an operation of the second type with $a = 2$. The resulting debts are: $d(1, 2) = 5$, $d(1, 3) = 5$, all other debts are $0$. </li></ol><p>In the second example the optimal sequence of operations can be the following:</p><ol> <li> Perform an operation of the first type with $a = 1$, $b = 2$, $c = 3$, $d = 1$ and $z = 10$. The resulting debts are: $d(3, 2) = 10$, $d(2, 3) = 15$, $d(1, 1) = 10$, all other debts are $0$; </li><li> Perform an operation of the first type with $a = 2$, $b = 3$, $c = 3$, $d = 2$ and $z = 10$. The resulting debts are: $d(2, 2) = 10$, $d(3, 3) = 10$, $d(2, 3) = 5$, $d(1, 1) = 10$, all other debts are $0$; </li><li> Perform an operation of the second type with $a = 2$. The resulting debts are: $d(3, 3) = 10$, $d(2, 3) = 5$, $d(1, 1) = 10$, all other debts are $0$; </li><li> Perform an operation of the second type with $a = 3$. The resulting debts are: $d(2, 3) = 5$, $d(1, 1) = 10$, all other debts are $0$; </li><li> Perform an operation of the second type with $a = 1$. The resulting debts are: $d(2, 3) = 5$, all other debts are $0$. </li></ol>
