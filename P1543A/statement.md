## Description

<div><p>Welcome to Rockport City!</p><p>It is time for your first ever race in the game against Ronnie. To make the race interesting, you have bet $a$ dollars and Ronnie has bet $b$ dollars. But the fans seem to be disappointed. The excitement of the fans is given by $gcd(a,b)$, where $gcd(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$. To make the race more exciting, you can perform two types of operations:</p><ol> <li> Increase both $a$ and $b$ by $1$. </li><li> Decrease both $a$ and $b$ by $1$. This operation can only be performed if both $a$ and $b$ are greater than $0$. </li></ol><p>In one move, you can perform any one of these operations. You can perform arbitrary (possibly zero) number of moves. Determine the maximum excitement the fans can get and the minimum number of moves required to achieve it.</p><p>Note that $gcd(x,0)=x$ for any $x \ge 0$.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1\leq t\leq 5\cdot 10^3$) — the number of test cases.</p><p>The first and the only line of each test case contains two integers $a$ and $b$ ($0\leq a, b\leq 10^{18}$).</p></div><div class="output-specification"><p>For each test case, print a single line containing two integers. </p><p>If the fans can get infinite excitement, print <span class="tex-font-style-tt">0 0</span>.</p><p>Otherwise, the first integer must be the maximum excitement the fans can get, and the second integer must be the minimum number of moves required to achieve that excitement.</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1\leq t\leq 5\cdot 10^3$) — the number of test cases.</p><p>The first and the only line of each test case contains two integers $a$ and $b$ ($0\leq a, b\leq 10^{18}$).</p>

## Output

<p>For each test case, print a single line containing two integers. </p><p>If the fans can get infinite excitement, print <span class="tex-font-style-tt">0 0</span>.</p><p>Otherwise, the first integer must be the maximum excitement the fans can get, and the second integer must be the minimum number of moves required to achieve that excitement.</p>





```input1
4
8 5
1 2
4 4
3 9
```




```output1
3 1
1 0
0 0
6 3
```



## Note

<p>For the first test case, you can apply the first operation $1$ time to get $a=9$ and $b=6$. It can be shown that $3$ is the maximum excitement possible.</p><p>For the second test case, no matter how many operations you apply, the fans will always have an excitement equal to $1$. Since the initial excitement is also $1$, you don't need to apply any operation.</p><p>For the third case, the fans can get infinite excitement by applying the first operation an infinite amount of times.</p><p>For the fourth test case, you can apply the second operation $3$ times to get $a=0$ and $b=6$. Since, $gcd(0,6)=6$, the fans will get an excitement of $6$.</p>
