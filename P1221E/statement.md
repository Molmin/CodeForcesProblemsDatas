## Description

<div><p>Alice and Bob play a game. Initially they have a string $s_1, s_2, \dots, s_n$, consisting of only characters <span class="tex-font-style-tt">.</span> and <span class="tex-font-style-tt">X</span>. They take alternating turns, and Alice is moving first. During each turn, the player has to select a contiguous substring consisting only of characters <span class="tex-font-style-tt">.</span> and replaces each of them with <span class="tex-font-style-tt">X</span>. Alice must select a substing of length $a$, and Bob must select a substring of length $b$. It is guaranteed that $a &gt; b$.</p><p>For example, if $s =$ <span class="tex-font-style-tt">...X..</span> and $a = 3$, $b = 2$, then after Alice's move string can turn only into <span class="tex-font-style-tt">XXXX..</span>. And if it's Bob's turn and the string $s =$ <span class="tex-font-style-tt">...X..</span>, then after Bob's move the string can turn into <span class="tex-font-style-tt">XX.X..</span>, <span class="tex-font-style-tt">.XXX..</span> or <span class="tex-font-style-tt">...XXX</span>.</p><p>Whoever is unable to make a move, loses. You have to determine who wins if they both play optimally.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line contains one integer $q$ ($1 \le q \le 3 \cdot 10^5$) — the number of queries.</p><p>The first line of each query contains two integers $a$ and $b$ ($1 \le b &lt; a \le 3 \cdot 10^5$).</p><p>The second line of each query contains the string $s$ ($1 \le |s| \le 3 \cdot 10^5$), consisting of only characters <span class="tex-font-style-tt">.</span> and <span class="tex-font-style-tt">X</span>.</p><p>It is guaranteed that sum of all $|s|$ over all queries not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case print <span class="tex-font-style-tt">YES</span> if Alice can win and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p></div>

## Input

<p>The first line contains one integer $q$ ($1 \le q \le 3 \cdot 10^5$) — the number of queries.</p><p>The first line of each query contains two integers $a$ and $b$ ($1 \le b &lt; a \le 3 \cdot 10^5$).</p><p>The second line of each query contains the string $s$ ($1 \le |s| \le 3 \cdot 10^5$), consisting of only characters <span class="tex-font-style-tt">.</span> and <span class="tex-font-style-tt">X</span>.</p><p>It is guaranteed that sum of all $|s|$ over all queries not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case print <span class="tex-font-style-tt">YES</span> if Alice can win and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print every letter in any case you want (so, for example, the strings <span class="tex-font-style-tt">yEs</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">Yes</span> and <span class="tex-font-style-tt">YES</span> will all be recognized as positive answer).</p>





```input1
3
3 2
XX......XX...X
4 2
X...X.X..X
5 3
.......X..X
```




```output1
YES
NO
YES
```



## Note

<p>In the first query Alice can select substring $s_3 \dots s_5$. After that $s$ turns into <span class="tex-font-style-tt">XXXXX...XX...X</span>. After that, no matter what move Bob makes, Alice can make the move (this will be her second move), but Bob can't make his second move.</p><p>In the second query Alice can not win because she cannot even make one move.</p><p>In the third query Alice can choose substring $s_2 \dots s_6$. After that $s$ turns into <span class="tex-font-style-tt">.XXXXX.X..X</span>, and Bob can't make a move after that.</p>
