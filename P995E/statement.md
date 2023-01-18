## Description

<div><p>Allen is playing Number Clicker on his phone.</p><p>He starts with an integer $u$ on the screen. Every second, he can press one of 3 buttons.</p><ol> <li> Turn $u \to u+1 \pmod{p}$. </li><li> Turn $u \to u+p-1 \pmod{p}$. </li><li> Turn $u \to u^{p-2} \pmod{p}$. </li></ol><p>Allen wants to press at most 200 buttons and end up with $v$ on the screen. Help him!</p></div><div class="input-specification"><p>The first line of the input contains 3 positive integers: $u, v, p$ ($0 \le u, v \le p-1$, $3 \le p \le 10^9 + 9$). $p$ is guaranteed to be prime.</p></div><div class="output-specification"><p>On the first line, print a single integer $\ell$, the number of button presses. On the second line, print integers $c_1, \dots, c_\ell$, the button presses. For $1 \le i \le \ell$, $1 \le c_i \le 3$.</p><p>We can show that the answer always exists.</p></div>

## Input

<p>The first line of the input contains 3 positive integers: $u, v, p$ ($0 \le u, v \le p-1$, $3 \le p \le 10^9 + 9$). $p$ is guaranteed to be prime.</p>

## Output

<p>On the first line, print a single integer $\ell$, the number of button presses. On the second line, print integers $c_1, \dots, c_\ell$, the button presses. For $1 \le i \le \ell$, $1 \le c_i \le 3$.</p><p>We can show that the answer always exists.</p>





```input1
1 3 5

```




```input2
3 2 5

```




```output1
2
1 1

```




```output2
1
3

```



## Note

<p>In the first example the integer on the screen changes as $1 \to 2 \to 3$.</p><p>In the second example the integer on the screen changes as $3 \to 2$. </p>
