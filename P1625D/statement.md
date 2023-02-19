## Description

<div><p>Binary Spiders are species of spiders that live on Mars. These spiders weave their webs to defend themselves from enemies.</p><p>To weave a web, spiders join in pairs. If the first spider in pair has $x$ legs, and the second spider has $y$ legs, then they weave a web with <span class="tex-font-style-it">durability</span> $x \oplus y$. Here, $\oplus$ means bitwise XOR.</p><p>Binary Spiders live in large groups. You observe a group of $n$ spiders, and the $i$-th spider has $a_i$ legs.</p><p>When the group is threatened, some of the spiders become <span class="tex-font-style-it">defenders</span>. Defenders are chosen in the following way. First, there must be at least two defenders. Second, any pair of defenders must be able to weave a web with durability at least $k$. Third, there must be as much defenders as possible.</p><p>Scientists have researched the behaviour of Binary Spiders for a long time, and now they have a hypothesis that they can always choose the defenders in an optimal way, satisfying the conditions above. You need to verify this hypothesis on your group of spiders. So, you need to understand how many spiders must become defenders. You are not a Binary Spider, so you decided to use a computer to solve this problem.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($2 \le n \le 3\cdot10^5$, $0 \le k \le 2^{30} - 1$), the amount of spiders in the group and the minimal allowed durability of a web.</p><p>The second line contains $n$ integers $a_i$ ($0 \le a_i \le 2^{30}-1$) — the number of legs the $i$-th spider has.</p></div><div class="output-specification"><p>In the first line, print a single integer $\ell$ ($2 \le \ell \le n$), the maximum possible amount of defenders.</p><p>In the second line, print $\ell$ integers $b_i$, separated by a single space ($1 \le b_i \le n$) — indices of spiders that will become defenders.</p><p>If there exists more than one way to choose the defenders, print any of them.</p><p>Unfortunately, it may appear that it's impossible to choose the defenders. In this case, print a single integer $-1$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($2 \le n \le 3\cdot10^5$, $0 \le k \le 2^{30} - 1$), the amount of spiders in the group and the minimal allowed durability of a web.</p><p>The second line contains $n$ integers $a_i$ ($0 \le a_i \le 2^{30}-1$) — the number of legs the $i$-th spider has.</p>

## Output

<p>In the first line, print a single integer $\ell$ ($2 \le \ell \le n$), the maximum possible amount of defenders.</p><p>In the second line, print $\ell$ integers $b_i$, separated by a single space ($1 \le b_i \le n$) — indices of spiders that will become defenders.</p><p>If there exists more than one way to choose the defenders, print any of them.</p><p>Unfortunately, it may appear that it's impossible to choose the defenders. In this case, print a single integer $-1$.</p>





```input1
6 8
2 8 4 16 10 14
```




```input2
6 1024
1 2 3 1 4 0
```




```output1
3
1 5 4
```




```output2
-1
```



## Note

<p>Consider the examples above.</p><p>In the first example, the group of spiders is illustrated on the picture below:</p><center> <img class="tex-graphics" src="file://03SCYGmf.png" style="max-width: 100.0%;max-height: 100.0%;" width="284px"> </center><p>We choose the two-legged, the ten-legged and the $16$-legged spiders. It's not hard to see that each pair may weave a web with enough durability, as $2 \oplus 10 = 8 \ge 8$, $2 \oplus 16 = 18 \ge 8$ and $10 \oplus 16 = 26 \ge 8$.</p><p>This is not the only way, as you can also choose, for example, the spiders with indices $3$, $4$, and $6$.</p><p>In the second example, no pair of spiders can weave the web with durability $1024$ or more, so the answer is $-1$.</p>
