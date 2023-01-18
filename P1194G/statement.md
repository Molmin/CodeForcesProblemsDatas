## Description

<div><p>Let's call a fraction $\frac{x}{y}$ good if there exists at least one another fraction $\frac{x'}{y'}$ such that $\frac{x}{y} = \frac{x'}{y'}$, $1 \le x', y' \le 9$, the digit denoting $x'$ is contained in the decimal representation of $x$, and the digit denoting $y'$ is contained in the decimal representation of $y$. For example, $\frac{26}{13}$ is a good fraction, because $\frac{26}{13} = \frac{2}{1}$.</p><p>You are given an integer number $n$. Please calculate the number of good fractions $\frac{x}{y}$ such that $1 \le x \le n$ and $1 \le y \le n$. The answer may be really large, so print it modulo $998244353$.</p></div><div class="input-specification"><p>The only line of the input contains one integer $n$ ($1 \le n &lt; 10^{100}$).</p></div><div class="output-specification"><p>Print the number of good fractions $\frac{x}{y}$ such that $1 \le x \le n$ and $1 \le y \le n$. The answer may be really large, so print it modulo $998244353$.</p></div>

## Input

<p>The only line of the input contains one integer $n$ ($1 \le n &lt; 10^{100}$).</p>

## Output

<p>Print the number of good fractions $\frac{x}{y}$ such that $1 \le x \le n$ and $1 \le y \le n$. The answer may be really large, so print it modulo $998244353$.</p>





```input1
42
```




```input2
3141592653589793238462643383279
```




```output1
150
```




```output2
459925407
```


