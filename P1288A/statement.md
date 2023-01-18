## Description

<div><p>Adilbek was assigned to a special project. For Adilbek it means that he has $n$ days to run a special program and provide its results. But there is a problem: the program needs to run for $d$ days to calculate the results.</p><p>Fortunately, Adilbek can optimize the program. If he spends $x$ ($x$ is a non-negative integer) days optimizing the program, he will make the program run in $\left\lceil \frac{d}{x + 1} \right\rceil$ days ($\left\lceil a \right\rceil$ is the ceiling function: $\left\lceil 2.4 \right\rceil = 3$, $\left\lceil 2 \right\rceil = 2$). The program cannot be run and optimized simultaneously, so the total number of days he will spend is equal to $x + \left\lceil \frac{d}{x + 1} \right\rceil$.</p><p>Will Adilbek be able to provide the generated results in no more than $n$ days?</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 50$) — the number of test cases.</p><p>The next $T$ lines contain test cases – one per line. Each line contains two integers $n$ and $d$ ($1 \le n \le 10^9$, $1 \le d \le 10^9$) — the number of days before the deadline and the number of days the program runs.</p></div><div class="output-specification"><p>Print $T$ answers — one per test case. For each test case print <span class="tex-font-style-tt">YES</span> (case insensitive) if Adilbek can fit in $n$ days or <span class="tex-font-style-tt">NO</span> (case insensitive) otherwise.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 50$) — the number of test cases.</p><p>The next $T$ lines contain test cases – one per line. Each line contains two integers $n$ and $d$ ($1 \le n \le 10^9$, $1 \le d \le 10^9$) — the number of days before the deadline and the number of days the program runs.</p>

## Output

<p>Print $T$ answers — one per test case. For each test case print <span class="tex-font-style-tt">YES</span> (case insensitive) if Adilbek can fit in $n$ days or <span class="tex-font-style-tt">NO</span> (case insensitive) otherwise.</p>





```input1
3
1 1
4 5
5 11
```




```output1
YES
YES
NO
```



## Note

<p>In the first test case, Adilbek decides not to optimize the program at all, since $d \le n$.</p><p>In the second test case, Adilbek can spend $1$ day optimizing the program and it will run $\left\lceil \frac{5}{2} \right\rceil = 3$ days. In total, he will spend $4$ days and will fit in the limit.</p><p>In the third test case, it's impossible to fit in the limit. For example, if Adilbek will optimize the program $2$ days, it'll still work $\left\lceil \frac{11}{2+1} \right\rceil = 4$ days.</p>
