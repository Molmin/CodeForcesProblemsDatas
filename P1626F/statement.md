## Description

<div><p>You are given an integer array $a_0, a_1, \dots, a_{n - 1}$, and an integer $k$. You perform the following code with it:</p><pre class="lstlisting"><code class="prettyprint">long long ans = 0; // create a 64-bit signed variable which is initially equal to 0<br>for(int i = 1; i &lt;= k; i++)<br>{<br>  int idx = rnd.next(0, n - 1); // generate a random integer between 0 and n - 1, both inclusive<br>                                // each integer from 0 to n - 1 has the same probability of being chosen<br>  ans += a[idx];<br>  a[idx] -= (a[idx] % i);<br>}<br></code></pre><p>Your task is to calculate the expected value of the variable <span class="tex-font-style-tt">ans</span> after performing this code.</p><p>Note that the input is generated according to special rules (see the input format section).</p></div><div class="input-specification"><p>The only line contains six integers $n$, $a_0$, $x$, $y$, $k$ and $M$ ($1 \le n \le 10^7$; $1 \le a_0, x, y &lt; M \le 998244353$; $1 \le k \le 17$).</p><p>The array $a$ in the input is constructed as follows:</p><ul> <li> $a_0$ is given in the input; </li><li> for every $i$ from $1$ to $n - 1$, the value of $a_i$ can be calculated as $a_i = (a_{i - 1} \cdot x + y) \bmod M$. </li></ul></div><div class="output-specification"><p>Let the expected value of the variable <span class="tex-font-style-tt">ans</span> after performing the code be $E$. It can be shown that $E \cdot n^k$ is an integer. You have to output this integer modulo $998244353$.</p></div>

## Input

<p>The only line contains six integers $n$, $a_0$, $x$, $y$, $k$ and $M$ ($1 \le n \le 10^7$; $1 \le a_0, x, y &lt; M \le 998244353$; $1 \le k \le 17$).</p><p>The array $a$ in the input is constructed as follows:</p><ul> <li> $a_0$ is given in the input; </li><li> for every $i$ from $1$ to $n - 1$, the value of $a_i$ can be calculated as $a_i = (a_{i - 1} \cdot x + y) \bmod M$. </li></ul>

## Output

<p>Let the expected value of the variable <span class="tex-font-style-tt">ans</span> after performing the code be $E$. It can be shown that $E \cdot n^k$ is an integer. You have to output this integer modulo $998244353$.</p>





```input1
3 10 3 5 13 88
```




```input2
2 15363 270880 34698 17 2357023
```




```output1
382842030
```




```output2
319392398
```



## Note

<p>The array in the first example test is $[10, 35, 22]$. In the second example, it is $[15363, 1418543]$.</p>
