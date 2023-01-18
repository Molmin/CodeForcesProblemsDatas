## Description

<div><p>Let $n$ be a positive integer. Let $a, b, c$ be nonnegative integers such that $a + b + c = n$.</p><p>Alice and Bob are gonna play rock-paper-scissors $n$ times. Alice knows the sequences of hands that Bob will play. However, Alice has to play rock $a$ times, paper $b$ times, and scissors $c$ times.</p><p>Alice wins if she beats Bob in at least $\lceil \frac{n}{2} \rceil$ ($\frac{n}{2}$ rounded up to the nearest integer) hands, otherwise Alice loses.</p><p>Note that in rock-paper-scissors:</p><ul> <li> rock beats scissors; </li><li> paper beats rock; </li><li> scissors beat paper. </li></ul><p>The task is, given the sequence of hands that Bob will play, and the numbers $a, b, c$, determine whether or not Alice can win. And if so, find any possible sequence of hands that Alice can use to win.</p><p>If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Then, $t$ testcases follow, each consisting of three lines: </p><ul> <li> The first line contains a single integer $n$ ($1 \le n \le 100$). </li><li> The second line contains three integers, $a, b, c$ ($0 \le a, b, c \le n$). It is guaranteed that $a + b + c = n$. </li><li> The third line contains a string $s$ of length $n$. $s$ is made up of only '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">P</span>', and '<span class="tex-font-style-tt">S</span>'. The $i$-th character is '<span class="tex-font-style-tt">R</span>' if for his $i$-th Bob plays rock, '<span class="tex-font-style-tt">P</span>' if paper, and '<span class="tex-font-style-tt">S</span>' if scissors. </li></ul></div><div class="output-specification"><p>For each testcase: </p><ul> <li> If Alice cannot win, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). </li><li> Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes). Also, print a string $t$ of length $n$ made up of only '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">P</span>', and '<span class="tex-font-style-tt">S</span>' — a sequence of hands that Alice can use to win. $t$ must contain exactly $a$ '<span class="tex-font-style-tt">R</span>'s, $b$ '<span class="tex-font-style-tt">P</span>'s, and $c$ '<span class="tex-font-style-tt">S</span>'s. </li><li> If there are multiple answers, print any of them. </li></ul><p>The "<span class="tex-font-style-tt">YES</span>" / "<span class="tex-font-style-tt">NO</span>" part of the output is case-insensitive (i.e. "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">no</span>" or "<span class="tex-font-style-tt">YEs</span>" are all valid answers). Note that '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">P</span>' and '<span class="tex-font-style-tt">S</span>' are case-sensitive.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$) — the number of test cases.</p><p>Then, $t$ testcases follow, each consisting of three lines: </p><ul> <li> The first line contains a single integer $n$ ($1 \le n \le 100$). </li><li> The second line contains three integers, $a, b, c$ ($0 \le a, b, c \le n$). It is guaranteed that $a + b + c = n$. </li><li> The third line contains a string $s$ of length $n$. $s$ is made up of only '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">P</span>', and '<span class="tex-font-style-tt">S</span>'. The $i$-th character is '<span class="tex-font-style-tt">R</span>' if for his $i$-th Bob plays rock, '<span class="tex-font-style-tt">P</span>' if paper, and '<span class="tex-font-style-tt">S</span>' if scissors. </li></ul>

## Output

<p>For each testcase: </p><ul> <li> If Alice cannot win, print "<span class="tex-font-style-tt">NO</span>" (without the quotes). </li><li> Otherwise, print "<span class="tex-font-style-tt">YES</span>" (without the quotes). Also, print a string $t$ of length $n$ made up of only '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">P</span>', and '<span class="tex-font-style-tt">S</span>' — a sequence of hands that Alice can use to win. $t$ must contain exactly $a$ '<span class="tex-font-style-tt">R</span>'s, $b$ '<span class="tex-font-style-tt">P</span>'s, and $c$ '<span class="tex-font-style-tt">S</span>'s. </li><li> If there are multiple answers, print any of them. </li></ul><p>The "<span class="tex-font-style-tt">YES</span>" / "<span class="tex-font-style-tt">NO</span>" part of the output is case-insensitive (i.e. "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">no</span>" or "<span class="tex-font-style-tt">YEs</span>" are all valid answers). Note that '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">P</span>' and '<span class="tex-font-style-tt">S</span>' are case-sensitive.</p>





```input1
2
3
1 1 1
RPS
3
3 0 0
RPS
```




```output1
YES
PSR
NO
```



## Note

<p>In the first testcase, in the first hand, Alice plays paper and Bob plays rock, so Alice beats Bob. In the second hand, Alice plays scissors and Bob plays paper, so Alice beats Bob. In the third hand, Alice plays rock and Bob plays scissors, so Alice beats Bob. Alice beat Bob 3 times, and $3 \ge \lceil \frac{3}{2} \rceil = 2$, so Alice wins.</p><p>In the second testcase, the only sequence of hands that Alice can play is "<span class="tex-font-style-tt">RRR</span>". Alice beats Bob only in the last hand, so Alice can't win. $1 &lt; \lceil \frac{3}{2} \rceil = 2$.</p>
