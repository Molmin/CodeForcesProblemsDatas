## Description

<div><p>Madoka wants to enter to "<span class="tex-font-style-it">Novosibirsk State University</span>", but in the entrance exam she came across a very difficult task:</p><p>Given an integer $n$, it is required to calculate $\sum{\operatorname{lcm}(c, \gcd(a, b))}$, for all triples of positive integers $(a, b, c)$, where $a + b + c = n$.</p><p>In this problem $\gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor</a> of $x$ and $y$, and $\operatorname{lcm}(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple</a> of $x$ and $y$.</p><p>Solve this problem for Madoka and help her to enter to the best university!</p></div><div class="input-specification"><p>The first and the only line contains a single integer $n$ ($3 \le n \le 10^5$).</p></div><div class="output-specification"><p>Print exactly one interger&nbsp;— $\sum{\operatorname{lcm}(c, \gcd(a, b))}$. Since the answer can be very large, then output it modulo $10^9 + 7$.</p></div>

## Input

<p>The first and the only line contains a single integer $n$ ($3 \le n \le 10^5$).</p>

## Output

<p>Print exactly one interger&nbsp;— $\sum{\operatorname{lcm}(c, \gcd(a, b))}$. Since the answer can be very large, then output it modulo $10^9 + 7$.</p>





```input1
3
```




```input2
5
```




```input3
69228
```




```output1
1
```




```output2
11
```




```output3
778304278
```



## Note

<p>In the first example, there is only one suitable triple $(1, 1, 1)$. So the answer is $\operatorname{lcm}(1, \gcd(1, 1)) = \operatorname{lcm}(1, 1) = 1$.</p><p>In the second example, $\operatorname{lcm}(1, \gcd(3, 1)) + \operatorname{lcm}(1, \gcd(2, 2)) + \operatorname{lcm}(1, \gcd(1, 3)) + \operatorname{lcm}(2, \gcd(2, 1)) + \operatorname{lcm}(2, \gcd(1, 2)) + \operatorname{lcm}(3, \gcd(1, 1)) = \operatorname{lcm}(1, 1) + \operatorname{lcm}(1, 2) + \operatorname{lcm}(1, 1) + \operatorname{lcm}(2, 1) + \operatorname{lcm}(2, 1) + \operatorname{lcm}(3, 1) = 1 + 2 + 1 + 2 + 2 + 3 = 11$</p>
