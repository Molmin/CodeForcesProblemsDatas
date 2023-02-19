## Description

<div><p>Christmas is coming, Icy has just received a box of chocolates from her grandparents! The box contains $n$ chocolates. The $i$-th chocolate has a non-negative integer type $a_i$.</p><p>Icy believes that good things come in pairs. Unfortunately, all types of chocolates are distinct (all $a_i$ are <span class="tex-font-style-bf">distinct</span>). Icy wants to make at least one pair of chocolates the same type. </p><p>As a result, she asks her grandparents to perform some <span class="tex-font-style-it">chocolate exchanges</span>. <span class="tex-font-style-bf">Before performing any chocolate exchanges</span>, Icy chooses two chocolates with indices $x$ and $y$ ($1 \le x, y \le n$, $x \ne y$).</p><p>In a <span class="tex-font-style-it">chocolate exchange</span>, Icy's grandparents choose a non-negative integer $k$, such that $2^k \ge a_x$, and change the type of the chocolate $x$ from $a_x$ to $2^k - a_x$ (that is, perform $a_x := 2^k - a_x$).</p><p>The chocolate exchanges will be stopped only when $a_x = a_y$. <span class="tex-font-style-bf">Note that other pairs of equal chocolate types do not stop the procedure.</span></p><p>Icy's grandparents are smart, so they would choose the sequence of chocolate exchanges that <span class="tex-font-style-bf">minimizes</span> the number of exchanges needed. Since Icy likes causing trouble, she wants to <span class="tex-font-style-bf">maximize</span> the minimum number of exchanges needed by choosing $x$ and $y$ appropriately. She wonders what is the optimal pair $(x, y)$ such that the minimum number of exchanges needed is maximized across all possible choices of $(x, y)$.</p><p>Since Icy is not good at math, she hopes that you can help her solve the problem.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of chocolates.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p><p>It is guaranteed that all $a_i$ are distinct.</p></div><div class="output-specification"><p>Output three integers $x$, $y$, and $m$.</p><p>$x$ and $y$ are indices of the optimal chocolates to perform exchanges on. Your output must satisfy $1 \le x, y \le n$, $x \ne y$.</p><p>$m$ is the number of exchanges needed to obtain $a_x = a_y$. We can show that $m \le 10^9$ for any pair of chocolates.</p><p>If there are multiple solutions, output any.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of chocolates.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 10^9$).</p><p>It is guaranteed that all $a_i$ are distinct.</p>

## Output

<p>Output three integers $x$, $y$, and $m$.</p><p>$x$ and $y$ are indices of the optimal chocolates to perform exchanges on. Your output must satisfy $1 \le x, y \le n$, $x \ne y$.</p><p>$m$ is the number of exchanges needed to obtain $a_x = a_y$. We can show that $m \le 10^9$ for any pair of chocolates.</p><p>If there are multiple solutions, output any.</p>





```input1
5
5 6 7 8 9
```




```input2
2
4 8
```




```output1
2 5 5
```




```output2
1 2 2
```



## Note

<p>In the first test case, the minimum number of exchanges needed to exchange a chocolate of type $6$ to a chocolate of type $9$ is $5$. The sequence of exchanges is as follows: $6 \rightarrow 2 \rightarrow 0 \rightarrow 1 \rightarrow 7 \rightarrow 9$.</p><p>In the second test case, the minimum number of exchanges needed to exchange a chocolate of type $4$ to a chocolate of type $8$ is $2$. The sequence of exchanges is as follows: $4 \rightarrow 0 \rightarrow 8$.</p>
