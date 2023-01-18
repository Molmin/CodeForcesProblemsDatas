## Description

<div><div class="epigraph"><div class="epigraph-text">Colossal!&nbsp;— exclaimed Hawk-nose.&nbsp;— A programmer! That's exactly what we are looking for.</div><div class="epigraph-source">Arkadi and Boris Strugatsky. Monday starts on Saturday</div></div><p>Reading the book "Equations of Mathematical Magic" Roman Oira-Oira and Cristobal Junta found an interesting equation: $a - (a \oplus x) - x = 0$ for some given $a$, where $\oplus$ stands for a bitwise exclusive or (XOR) of two integers (this operation is denoted as <span class="tex-font-style-tt">^</span> or <span class="tex-font-style-tt">xor</span> in many modern programming languages). Oira-Oira quickly found some $x$, which is the solution of the equation, but Cristobal Junta decided that Oira-Oira's result is not interesting enough, so he asked his colleague how many <span class="tex-font-style-bf">non-negative</span> solutions of this equation exist. This task turned out to be too difficult for Oira-Oira, so he asks you to help.</p></div><div class="input-specification"><p>Each test contains several possible values of $a$ and your task is to find the number of equation's solution for each of them. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of these values.</p><p>The following $t$ lines contain the values of parameter $a$, each value is an integer from $0$ to $2^{30} - 1$ inclusive.</p></div><div class="output-specification"><p>For each value of $a$ print exactly one integer&nbsp;— the number of non-negative solutions of the equation for the given value of the parameter. Print answers in the same order as values of $a$ appear in the input.</p><p>One can show that the number of solutions is always finite.</p></div>

## Input

<p>Each test contains several possible values of $a$ and your task is to find the number of equation's solution for each of them. The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of these values.</p><p>The following $t$ lines contain the values of parameter $a$, each value is an integer from $0$ to $2^{30} - 1$ inclusive.</p>

## Output

<p>For each value of $a$ print exactly one integer&nbsp;— the number of non-negative solutions of the equation for the given value of the parameter. Print answers in the same order as values of $a$ appear in the input.</p><p>One can show that the number of solutions is always finite.</p>





```input1
3
0
2
1073741823

```




```output1
1
2
1073741824

```



## Note

<p>Let's define the bitwise exclusive OR (XOR) operation. Given two integers $x$ and $y$, consider their binary representations (possibly with leading zeroes): $x_k \dots x_2 x_1 x_0$ and $y_k \dots y_2 y_1 y_0$. Here, $x_i$ is the $i$-th bit of the number $x$ and $y_i$ is the $i$-th bit of the number $y$. Let $r = x \oplus y$ be the result of the XOR operation of $x$ and $y$. Then $r$ is defined as $r_k \dots r_2 r_1 r_0$ where:</p><p>$$ r_i = \left\{ \begin{aligned} 1, ~ \text{if} ~ x_i \ne y_i \\ 0, ~ \text{if} ~ x_i = y_i \end{aligned} \right. $$</p><p>For the first value of the parameter, only $x = 0$ is a solution of the equation.</p><p>For the second value of the parameter, solutions are $x = 0$ and $x = 2$.</p>
