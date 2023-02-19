## Description

<div><p>Vlad came home and found out that someone had reconfigured the old thermostat to the temperature of $a$.</p><p>The thermostat can only be set to a temperature from $l$ to $r$ inclusive, the temperature cannot change by less than $x$. Formally, in one operation you can reconfigure the thermostat from temperature $a$ to temperature $b$ if $|a - b| \ge x$ and $l \le b \le r$.</p><p>You are given $l$, $r$, $x$, $a$ and $b$. Find the minimum number of operations required to get temperature $b$ from temperature $a$, or say that it is impossible.</p></div><div class="input-specification"><p>The first line of input data contains the single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each case contains three integers $l$, $r$ and $x$ ($-10^9 \le l \le r \le 10^9$, $1 \le x \le 10^9$) — range of temperature and minimum temperature change.</p><p>The second line of each case contains two integers $a$ and $b$ ($l \le a, b \le r$) — the initial and final temperatures.</p></div><div class="output-specification"><p>Output $t$ numbers, each of which is the answer to the corresponding test case. If it is impossible to achieve the temperature $b$, output <span class="tex-font-style-tt">-1</span>, otherwise output the minimum number of operations.</p></div>

## Input

<p>The first line of input data contains the single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test.</p><p>The descriptions of the test cases follow.</p><p>The first line of each case contains three integers $l$, $r$ and $x$ ($-10^9 \le l \le r \le 10^9$, $1 \le x \le 10^9$) — range of temperature and minimum temperature change.</p><p>The second line of each case contains two integers $a$ and $b$ ($l \le a, b \le r$) — the initial and final temperatures.</p>

## Output

<p>Output $t$ numbers, each of which is the answer to the corresponding test case. If it is impossible to achieve the temperature $b$, output <span class="tex-font-style-tt">-1</span>, otherwise output the minimum number of operations.</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
3 5 6
3 3
0 15 5
4 5
0 10 5
3 7
3 5 6
3 4
-10 10 11
-5 6
-3 3 4
1 0
-5 10 8
9 2
1 5 1
2 5
-1 4 3
0 2
-6 3 6
-1 -4
```




```output1
0
2
3
-1
1
-1
3
1
3
-1
```



## Note

<p>In the first example, the thermostat is already set up correctly.</p><p>In the second example, you can achieve the desired temperature as follows: $4 \rightarrow 10 \rightarrow 5$.</p><p>In the third example, you can achieve the desired temperature as follows: $3 \rightarrow 8 \rightarrow 2 \rightarrow 7$.</p><p>In the fourth test, it is impossible to make any operation.</p>
