## Description

<div><p>Consider the array $a$ composed of all the integers in the range $[l, r]$. For example, if $l = 3$ and $r = 7$, then $a = [3, 4, 5, 6, 7]$.</p><p>Given $l$, $r$, and $k$, is it possible for $\gcd(a)$ to be greater than $1$ after doing the following operation at most $k$ times? </p><ul> <li> Choose $2$ numbers from $a$. </li><li> Permanently remove one occurrence of each of them from the array. </li><li> Insert their product back into $a$. </li></ul><p>$\gcd(b)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of the integers in $b$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. The description of test cases follows.</p><p>The input for each test case consists of a single line containing $3$ non-negative integers $l$, $r$, and $k$ ($1 \leq l \leq r \leq 10^9, \enspace 0 \leq k \leq r - l$).</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if it is possible to have the GCD of the corresponding array greater than $1$ by performing at most $k$ operations, and "<span class="tex-font-style-tt">NO</span>" otherwise (case insensitive).</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 10^5$) — the number of test cases. The description of test cases follows.</p><p>The input for each test case consists of a single line containing $3$ non-negative integers $l$, $r$, and $k$ ($1 \leq l \leq r \leq 10^9, \enspace 0 \leq k \leq r - l$).</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>" if it is possible to have the GCD of the corresponding array greater than $1$ by performing at most $k$ operations, and "<span class="tex-font-style-tt">NO</span>" otherwise (case insensitive).</p>





```input1
9
1 1 0
3 5 1
13 13 0
4 4 0
3 7 4
4 10 3
2 4 0
1 7 3
1 5 3
```




```output1
NO
NO
YES
YES
YES
YES
NO
NO
YES
```



## Note

<p>For the first test case, $a = [1]$, so the answer is "<span class="tex-font-style-tt">NO</span>", since the only element in the array is $1$.</p><p>For the second test case the array is $a = [3, 4, 5]$ and we have $1$ operation. After the first operation the array can change to: $[3, 20]$, $[4, 15]$ or $[5, 12]$ all of which having their greatest common divisor equal to $1$ so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>For the third test case, $a = [13]$, so the answer is "<span class="tex-font-style-tt">YES</span>", since the only element in the array is $13$.</p><p>For the fourth test case, $a = [4]$, so the answer is "<span class="tex-font-style-tt">YES</span>", since the only element in the array is $4$.</p>
