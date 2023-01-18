## Description

<div><p>While discussing a proper problem A for a Codeforces Round, Kostya created a cyclic array of positive integers $a_1, a_2, \ldots, a_n$. Since the talk was long and not promising, Kostya created a new cyclic array $b_1, b_2, \ldots, b_{n}$ so that $b_i = (a_i \mod a_{i + 1})$, where we take $a_{n+1} = a_1$. Here $mod$ is the <a href="https://en.wikipedia.org/wiki/Modulo_operation">modulo operation</a>. When the talk became interesting, Kostya completely forgot how array $a$ had looked like. Suddenly, he thought that restoring array $a$ from array $b$ would be an interesting problem (unfortunately, not A).</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 140582$) — the length of the array $a$.</p><p>The second line contains $n$ integers $b_1, b_2, \ldots, b_{n}$ ($0 \le b_i \le 187126$).</p></div><div class="output-specification"><p>If it is possible to restore some array $a$ of length $n$ so that $b_i = a_i \mod a_{(i \mod n) + 1}$ holds for all $i = 1, 2, \ldots, n$, print «<span class="tex-font-style-tt">YES</span>» in the first line and the integers $a_1, a_2, \ldots, a_n$ in the second line. All $a_i$ should satisfy $1 \le a_i \le 10^{18}$. We can show that if an answer exists, then an answer with such constraint exists as well.</p><p>It it impossible to restore any valid $a$, print «<span class="tex-font-style-tt">NO</span>» in one line.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 140582$) — the length of the array $a$.</p><p>The second line contains $n$ integers $b_1, b_2, \ldots, b_{n}$ ($0 \le b_i \le 187126$).</p>

## Output

<p>If it is possible to restore some array $a$ of length $n$ so that $b_i = a_i \mod a_{(i \mod n) + 1}$ holds for all $i = 1, 2, \ldots, n$, print «<span class="tex-font-style-tt">YES</span>» in the first line and the integers $a_1, a_2, \ldots, a_n$ in the second line. All $a_i$ should satisfy $1 \le a_i \le 10^{18}$. We can show that if an answer exists, then an answer with such constraint exists as well.</p><p>It it impossible to restore any valid $a$, print «<span class="tex-font-style-tt">NO</span>» in one line.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
1 3 1 0

```




```input2
2
4 4

```




```output1
YES
1 3 5 2

```




```output2
NO

```



## Note

<p>In the first example:</p><ul> <li> $1 \mod 3 = 1$ </li><li> $3 \mod 5 = 3$ </li><li> $5 \mod 2 = 1$ </li><li> $2 \mod 1 = 0$ </li></ul>
