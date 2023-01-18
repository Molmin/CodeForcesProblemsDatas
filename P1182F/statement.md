## Description

<div><p>You have given integers $a$, $b$, $p$, and $q$. Let $f(x) = \text{abs}(\text{sin}(\frac{p}{q} \pi x))$.</p><p>Find minimum possible integer $x$ that maximizes $f(x)$ where $a \le x \le b$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains four integers $a$, $b$, $p$, and $q$ ($0 \le a \le b \le 10^{9}$, $1 \le p$, $q \le 10^{9}$).</p></div><div class="output-specification"><p>Print the minimum possible integer $x$ for each test cases, separated by newline.</p></div>

## Input

<p>Each test contains multiple test cases. </p><p>The first line contains the number of test cases $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains four integers $a$, $b$, $p$, and $q$ ($0 \le a \le b \le 10^{9}$, $1 \le p$, $q \le 10^{9}$).</p>

## Output

<p>Print the minimum possible integer $x$ for each test cases, separated by newline.</p>





```input1
2
0 3 1 3
17 86 389 995
```




```output1
1
55
```



## Note

<p>In the first test case, $f(0) = 0$, $f(1) = f(2) \approx 0.866$, $f(3) = 0$.</p><p>In the second test case, $f(55) \approx 0.999969$, which is the largest among all possible values.</p>
