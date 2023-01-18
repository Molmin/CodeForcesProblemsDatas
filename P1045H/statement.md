## Description

<div><p>Being bored of exploring the Moon over and over again Wall-B decided to explore something he is made of — binary numbers. He took a binary number and decided to count how many times different substrings of length two appeared. He stored those values in $c_{00}$, $c_{01}$, $c_{10}$ and $c_{11}$, representing how many times substrings <span class="tex-font-style-tt">00</span>, <span class="tex-font-style-tt">01</span>, <span class="tex-font-style-tt">10</span> and <span class="tex-font-style-tt">11</span> appear in the number respectively. For example:</p><p> $10111100 \rightarrow c_{00} = 1, \ c_{01} = 1,\ c_{10} = 2,\ c_{11} = 3$</p><p> $10000 \rightarrow c_{00} = 3,\ c_{01} = 0,\ c_{10} = 1,\ c_{11} = 0$</p><p> $10101001 \rightarrow c_{00} = 1,\ c_{01} = 3,\ c_{10} = 3,\ c_{11} = 0$</p><p> $1 \rightarrow c_{00} = 0,\ c_{01} = 0,\ c_{10} = 0,\ c_{11} = 0$</p><p>Wall-B noticed that there can be multiple binary numbers satisfying the same $c_{00}$, $c_{01}$, $c_{10}$ and $c_{11}$ constraints. Because of that he wanted to count how many binary numbers satisfy the constraints $c_{xy}$ given the interval $[A, B]$. Unfortunately, his processing power wasn't strong enough to handle large intervals he was curious about. Can you help him? Since this number can be large print it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>First two lines contain two positive binary numbers $A$ and $B$ ($1 \leq A \leq B &lt; 2^{100\,000}$), representing the start and the end of the interval respectively. Binary numbers $A$ and $B$ have no leading zeroes.</p><p>Next four lines contain decimal numbers $c_{00}$, $c_{01}$, $c_{10}$ and $c_{11}$ ($0 \leq c_{00}, c_{01}, c_{10}, c_{11} \leq 100\,000$) representing the count of two-digit substrings <span class="tex-font-style-tt">00</span>, <span class="tex-font-style-tt">01</span>, <span class="tex-font-style-tt">10</span> and <span class="tex-font-style-tt">11</span> respectively. </p></div><div class="output-specification"><p>Output one integer number representing how many binary numbers in the interval $[A, B]$ satisfy the constraints mod $10^9 + 7$.</p></div>

## Input

<p>First two lines contain two positive binary numbers $A$ and $B$ ($1 \leq A \leq B &lt; 2^{100\,000}$), representing the start and the end of the interval respectively. Binary numbers $A$ and $B$ have no leading zeroes.</p><p>Next four lines contain decimal numbers $c_{00}$, $c_{01}$, $c_{10}$ and $c_{11}$ ($0 \leq c_{00}, c_{01}, c_{10}, c_{11} \leq 100\,000$) representing the count of two-digit substrings <span class="tex-font-style-tt">00</span>, <span class="tex-font-style-tt">01</span>, <span class="tex-font-style-tt">10</span> and <span class="tex-font-style-tt">11</span> respectively. </p>

## Output

<p>Output one integer number representing how many binary numbers in the interval $[A, B]$ satisfy the constraints mod $10^9 + 7$.</p>





```input1
10
1001
0
0
1
1

```




```input2
10
10001
1
2
3
4

```




```output1
1

```




```output2
0

```



## Note

<p>Example 1: The binary numbers in the interval $[10,1001]$ are $10,11,100,101,110,111,1000,1001$. Only number 110 satisfies the constraints: $c_{00} = 0, c_{01} = 0, c_{10} = 1, c_{11} = 1$.</p><p>Example 2: No number in the interval satisfies the constraints</p>
