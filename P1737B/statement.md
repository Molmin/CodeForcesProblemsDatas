## Description

<div><p></p><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-left"><img class="tex-graphics" src="file://9zz8fPPQ.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-left"><span class="tex-font-style-it">While working at DTL, Ela is very aware of her physical and mental health. She started to practice various sports, such as Archery, Yoga, and Football.</span></td></tr></tbody></table><p></p><p>Since she started engaging in sports activities, Ela switches to trying a new sport on days she considers being <span class="tex-font-style-it">"Luxury" days</span>. She counts the days since she started these activities, in which the day she starts is numbered as day $1$. A "Luxury" day is the day in which the number of this day is a <span class="tex-font-style-it">luxurious number</span>. </p><p>An integer $x$ is called a <span class="tex-font-style-it">luxurious number</span> if it is divisible by ${\lfloor \sqrt{x} \rfloor}$.</p><p>Here $\lfloor r \rfloor$ denotes the <span class="tex-font-style-tt">"floor"</span> of a real number $r$. In other words, it's the largest integer not greater than $r$.</p><p>For example: $8$, $56$, $100$ are <span class="tex-font-style-it">luxurious numbers</span>, since $8$ is divisible by $\lfloor \sqrt{8} \rfloor = \lfloor 2.8284 \rfloor = 2$, $56$ is divisible $\lfloor \sqrt{56} \rfloor = \lfloor 7.4833 \rfloor = 7$, and $100$ is divisible by $\lfloor \sqrt{100} \rfloor = \lfloor 10 \rfloor = 10$, respectively. On the other hand $5$, $40$ are not, since $5$ are not divisible by $\lfloor \sqrt{5} \rfloor = \lfloor 2.2361 \rfloor = 2$, and $40$ are not divisible by $\lfloor \sqrt{40} \rfloor = \lfloor 6.3246 \rfloor = 6$.</p><p>Being a friend of Ela, you want to engage in these fitness activities with her to keep her and yourself accompanied (and have fun together, of course). Between day $l$ and day $r$, you want to know how many times she changes the activities.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line has the number of test cases $t$ ($1 \le t \le 10\ 000$). The description of the test cases follows.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1 \le l \le r \le 10^{18}$) — the intervals at which you want to know how many times Ela changes her sports.</p></div><div class="output-specification"><p>For each test case, output an integer that denotes the answer.</p></div>

## Input

<p>Each test contains multiple test cases. The first line has the number of test cases $t$ ($1 \le t \le 10\ 000$). The description of the test cases follows.</p><p>The only line of each test case contains two integers $l$ and $r$ ($1 \le l \le r \le 10^{18}$) — the intervals at which you want to know how many times Ela changes her sports.</p>

## Output

<p>For each test case, output an integer that denotes the answer.</p>





```input1|2,4,6
5
8 19
8 20
119 121
1 100000000000000000
1234567891011 1000000000000000000
```




```output1
5
6
2
948683296
2996666667
```



## Note

<p>In the first test case, $5$ luxury numbers in range $[8, 19]$ are: $8, 9, 12, 15, 16$.</p>
