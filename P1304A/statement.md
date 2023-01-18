## Description

<div><p>Being tired of participating in too many Codeforces rounds, Gildong decided to take some rest in a park. He sat down on a bench, and soon he found two rabbits hopping around. One of the rabbits was taller than the other.</p><p>He noticed that the two rabbits were hopping <span class="tex-font-style-it">towards each other</span>. The positions of the two rabbits can be represented as integer coordinates on a horizontal line. The taller rabbit is currently on position $x$, and the shorter rabbit is currently on position $y$ ($x \lt y$). Every second, each rabbit hops to another position. The taller rabbit hops to the positive direction by $a$, and the shorter rabbit hops to the negative direction by $b$.</p><center> <img class="tex-graphics" src="file://NIWm465g.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For example, let's say $x=0$, $y=10$, $a=2$, and $b=3$. At the $1$-st second, each rabbit will be at position $2$ and $7$. At the $2$-nd second, both rabbits will be at position $4$.</p><p>Gildong is now wondering: <span class="tex-font-style-it">Will the two rabbits be at the same position <span class="tex-font-style-bf">at the same moment</span>? If so, how long will it take?</span> Let's find a moment in time (in seconds) after which the rabbits will be at the same point.</p></div><div class="input-specification"><p>Each test contains one or more test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$).</p><p>Each test case contains exactly one line. The line consists of four integers $x$, $y$, $a$, $b$ ($0 \le x \lt y \le 10^9$, $1 \le a,b \le 10^9$) — the current position of the taller rabbit, the current position of the shorter rabbit, the hopping distance of the taller rabbit, and the hopping distance of the shorter rabbit, respectively.</p></div><div class="output-specification"><p>For each test case, print the single integer: number of seconds the two rabbits will take to be at the same position.</p><p>If the two rabbits will never be at the same position simultaneously, print $-1$.</p></div>

## Input

<p>Each test contains one or more test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$).</p><p>Each test case contains exactly one line. The line consists of four integers $x$, $y$, $a$, $b$ ($0 \le x \lt y \le 10^9$, $1 \le a,b \le 10^9$) — the current position of the taller rabbit, the current position of the shorter rabbit, the hopping distance of the taller rabbit, and the hopping distance of the shorter rabbit, respectively.</p>

## Output

<p>For each test case, print the single integer: number of seconds the two rabbits will take to be at the same position.</p><p>If the two rabbits will never be at the same position simultaneously, print $-1$.</p>





```input1
5
0 10 2 3
0 10 3 3
900000000 1000000000 1 9999999
1 2 1 1
1 3 1 1
```




```output1
2
-1
10
-1
1
```



## Note

<p>The first case is explained in the description.</p><p>In the second case, each rabbit will be at position $3$ and $7$ respectively at the $1$-st second. But in the $2$-nd second they will be at $6$ and $4$ respectively, and we can see that they will never be at the same position since the distance between the two rabbits will only increase afterward.</p>
