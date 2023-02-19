## Description

<div><p>Monocarp is playing a computer game. In this game, his character fights different monsters.</p><p>A fight between a character and a monster goes as follows. Suppose the character initially has health $h_C$ and attack $d_C$; the monster initially has health $h_M$ and attack $d_M$. The fight consists of several steps:</p><ol> <li> the character attacks the monster, decreasing the monster's health by $d_C$; </li><li> the monster attacks the character, decreasing the character's health by $d_M$; </li><li> the character attacks the monster, decreasing the monster's health by $d_C$; </li><li> the monster attacks the character, decreasing the character's health by $d_M$; </li><li> and so on, until the end of the fight. </li></ol><p>The fight ends when someone's health becomes non-positive (i. e. $0$ or less). If the monster's health becomes non-positive, the character wins, otherwise the monster wins.</p><p>Monocarp's character currently has health equal to $h_C$ and attack equal to $d_C$. He wants to slay a monster with health equal to $h_M$ and attack equal to $d_M$. Before the fight, Monocarp can spend up to $k$ coins to upgrade his character's weapon and/or armor; each upgrade costs exactly one coin, each weapon upgrade increases the character's attack by $w$, and each armor upgrade increases the character's health by $a$.</p><p>Can Monocarp's character slay the monster if Monocarp spends coins on upgrades optimally?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5 \cdot 10^4$) — the number of test cases. Each test case consists of three lines:</p><p>The first line contains two integers $h_C$ and $d_C$ ($1 \le h_C \le 10^{15}$; $1 \le d_C \le 10^9$) — the character's health and attack;</p><p>The second line contains two integers $h_M$ and $d_M$ ($1 \le h_M \le 10^{15}$; $1 \le d_M \le 10^9$) — the monster's health and attack;</p><p>The third line contains three integers $k$, $w$ and $a$ ($0 \le k \le 2 \cdot 10^5$; $0 \le w \le 10^4$; $0 \le a \le 10^{10}$) — the maximum number of coins that Monocarp can spend, the amount added to the character's attack with each weapon upgrade, and the amount added to the character's health with each armor upgrade, respectively.</p><p>The sum of $k$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to slay the monster by optimally choosing the upgrades. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5 \cdot 10^4$) — the number of test cases. Each test case consists of three lines:</p><p>The first line contains two integers $h_C$ and $d_C$ ($1 \le h_C \le 10^{15}$; $1 \le d_C \le 10^9$) — the character's health and attack;</p><p>The second line contains two integers $h_M$ and $d_M$ ($1 \le h_M \le 10^{15}$; $1 \le d_M \le 10^9$) — the monster's health and attack;</p><p>The third line contains three integers $k$, $w$ and $a$ ($0 \le k \le 2 \cdot 10^5$; $0 \le w \le 10^4$; $0 \le a \le 10^{10}$) — the maximum number of coins that Monocarp can spend, the amount added to the character's attack with each weapon upgrade, and the amount added to the character's health with each armor upgrade, respectively.</p><p>The sum of $k$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">YES</span> if it is possible to slay the monster by optimally choosing the upgrades. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
4
25 4
9 20
1 1 10
25 4
12 20
1 1 10
100 1
45 2
0 4 10
9 2
69 2
4 2 7
```




```output1
YES
NO
YES
YES
```



## Note

<p>In the first example, Monocarp can spend one coin to upgrade weapon (damage will be equal to $5$), then health during battle will change as follows: $(h_C, h_M) = (25, 9) \rightarrow (25, 4) \rightarrow (5, 4) \rightarrow (5, -1)$. The battle ended with Monocarp's victory.</p><p>In the second example, Monocarp has no way to defeat the monster.</p><p>In the third example, Monocarp has no coins, so he can't buy upgrades. However, the initial characteristics are enough for Monocarp to win.</p><p>In the fourth example, Monocarp has $4$ coins. To defeat the monster, he has to spend $2$ coins to upgrade weapon and $2$ coins to upgrade armor.</p>
