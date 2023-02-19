## Description

<div><p>You are given three integers $n$, $k$ and $f$.</p><p>Consider all binary strings (i. e. all strings consisting of characters $0$ and/or $1$) of length from $1$ to $n$. For every such string $s$, you need to choose an integer $c_s$ from $0$ to $k$.</p><p>A multiset of binary strings of length <span class="tex-font-style-bf">exactly</span> $n$ is considered beautiful if for every binary string $s$ with length from $1$ to $n$, the number of strings in the multiset such that $s$ is their prefix is not exceeding $c_s$.</p><p>For example, let $n = 2$, $c_{0} = 3$, $c_{00} = 1$, $c_{01} = 2$, $c_{1} = 1$, $c_{10} = 2$, and $c_{11} = 3$. The multiset of strings $\{11, 01, 00, 01\}$ is beautiful, since:</p><ul> <li> for the string $0$, there are $3$ strings in the multiset such that $0$ is their prefix, and $3 \le c_0$; </li><li> for the string $00$, there is one string in the multiset such that $00$ is its prefix, and $1 \le c_{00}$; </li><li> for the string $01$, there are $2$ strings in the multiset such that $01$ is their prefix, and $2 \le c_{01}$; </li><li> for the string $1$, there is one string in the multiset such that $1$ is its prefix, and $1 \le c_1$; </li><li> for the string $10$, there are $0$ strings in the multiset such that $10$ is their prefix, and $0 \le c_{10}$; </li><li> for the string $11$, there is one string in the multiset such that $11$ is its prefix, and $1 \le c_{11}$. </li></ul><p>Now, for the problem itself. You have to calculate the number of ways to choose the integer $c_s$ for every binary string $s$ of length from $1$ to $n$ in such a way that the <span class="tex-font-style-bf">maximum</span> possible size of a beautiful multiset is <span class="tex-font-style-bf">exactly</span> $f$.</p></div><div class="input-specification"><p>The only line of input contains three integers $n$, $k$ and $f$ ($1 \le n \le 15$; $1 \le k, f \le 2 \cdot 10^5$).</p></div><div class="output-specification"><p>Print one integer — the number of ways to choose the integer $c_s$ for every binary string $s$ of length from $1$ to $n$ in such a way that the <span class="tex-font-style-bf">maximum</span> possible size of a beautiful multiset is <span class="tex-font-style-bf">exactly</span> $f$. Since it can be huge, print it modulo $998244353$.</p></div>

## Input

<p>The only line of input contains three integers $n$, $k$ and $f$ ($1 \le n \le 15$; $1 \le k, f \le 2 \cdot 10^5$).</p>

## Output

<p>Print one integer — the number of ways to choose the integer $c_s$ for every binary string $s$ of length from $1$ to $n$ in such a way that the <span class="tex-font-style-bf">maximum</span> possible size of a beautiful multiset is <span class="tex-font-style-bf">exactly</span> $f$. Since it can be huge, print it modulo $998244353$.</p>





```input1
1 42 2
```




```input2
2 37 13
```




```input3
4 1252 325
```




```input4
6 153 23699
```




```input5
15 200000 198756
```




```output1
3
```




```output2
36871576
```




```output3
861735572
```




```output4
0
```




```output5
612404746
```



## Note

<p>In the first example, the three ways to choose the integers $c_s$ are:</p><ul> <li> $c_0 = 0$, $c_1 = 2$, then the maximum beautiful multiset is $\{1, 1\}$; </li><li> $c_0 = 1$, $c_1 = 1$, then the maximum beautiful multiset is $\{0, 1\}$; </li><li> $c_0 = 2$, $c_1 = 0$, then the maximum beautiful multiset is $\{0, 0\}$. </li></ul>
