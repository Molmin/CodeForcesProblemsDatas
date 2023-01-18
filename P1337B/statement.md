## Description

<div><p>Kana was just an ordinary high school girl before a talent scout discovered her. Then, she became an idol. But different from the stereotype, she is also a gameholic. </p><p>One day Kana gets interested in a new adventure game called <span class="tex-font-style-it">Dragon Quest</span>. In this game, her quest is to beat a dragon.</p><center><img class="tex-graphics" src="file://4LdVFRkD.png" style="max-width: 100.0%;max-height: 100.0%;"></center>&nbsp;<p>The dragon has a <span class="tex-font-style-it">hit point</span> of $x$ initially. When its <span class="tex-font-style-it">hit point</span> goes to $0$ or under $0$, it will be defeated. In order to defeat the dragon, Kana can cast the two following types of spells. </p><ul><li> <span class="tex-font-style-tt">Void Absorption</span> <p>Assume that the dragon's current <span class="tex-font-style-it">hit point</span> is $h$, after <span class="tex-font-style-it">casting</span> this spell its <span class="tex-font-style-it">hit point</span> will become $\left\lfloor \frac{h}{2} \right\rfloor + 10$. Here $\left\lfloor \frac{h}{2} \right\rfloor$ denotes $h$ divided by two, rounded down.</p></li><li> <span class="tex-font-style-tt">Lightning Strike</span> <p>This spell will decrease the dragon's <span class="tex-font-style-it">hit point</span> by $10$. Assume that the dragon's current <span class="tex-font-style-it">hit point</span> is $h$, after <span class="tex-font-style-it">casting</span> this spell its <span class="tex-font-style-it">hit point</span> will be lowered to $h-10$.</p></li></ul><p>Due to some reasons Kana can only <span class="tex-font-style-it">cast</span> <span class="tex-font-style-bf">no more than</span> $n$ <span class="tex-font-style-tt">Void Absorptions</span> and $m$ <span class="tex-font-style-tt">Lightning Strikes</span>. She can cast the spells in any order and <span class="tex-font-style-bf">doesn't have to</span> cast all the spells. Kana isn't good at math, so you are going to help her to find out whether it is possible to defeat the dragon.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$) &nbsp;— the number of test cases.</p><p>The next $t$ lines describe test cases. For each test case the only line contains three integers $x$, $n$, $m$ ($1\le x \le 10^5$, $0\le n,m\le30$) &nbsp;— the dragon's intitial <span class="tex-font-style-it">hit point</span>, the maximum number of <span class="tex-font-style-tt">Void Absorptions</span> and <span class="tex-font-style-tt">Lightning Strikes</span> Kana can <span class="tex-font-style-it">cast</span> respectively.</p></div><div class="output-specification"><p>If it is possible to defeat the dragon, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 1000$) &nbsp;— the number of test cases.</p><p>The next $t$ lines describe test cases. For each test case the only line contains three integers $x$, $n$, $m$ ($1\le x \le 10^5$, $0\le n,m\le30$) &nbsp;— the dragon's intitial <span class="tex-font-style-it">hit point</span>, the maximum number of <span class="tex-font-style-tt">Void Absorptions</span> and <span class="tex-font-style-tt">Lightning Strikes</span> Kana can <span class="tex-font-style-it">cast</span> respectively.</p>

## Output

<p>If it is possible to defeat the dragon, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in any case (upper or lower).</p>





```input1
7
100 3 4
189 3 4
64 2 3
63 2 3
30 27 7
10 9 1
69117 21 2
```




```output1
YES
NO
NO
YES
YES
YES
YES
```



## Note

<p>One possible casting sequence of the first test case is shown below:</p><ul><li> <span class="tex-font-style-tt">Void Absorption</span> $\left\lfloor \frac{100}{2} \right\rfloor + 10=60$.</li><li> <span class="tex-font-style-tt">Lightning Strike</span> $60-10=50$.</li><li> <span class="tex-font-style-tt">Void Absorption</span> $\left\lfloor \frac{50}{2} \right\rfloor + 10=35$.</li><li> <span class="tex-font-style-tt">Void Absorption</span> $\left\lfloor \frac{35}{2} \right\rfloor + 10=27$.</li><li> <span class="tex-font-style-tt">Lightning Strike</span> $27-10=17$.</li><li> <span class="tex-font-style-tt">Lightning Strike</span> $17-10=7$.</li><li> <span class="tex-font-style-tt">Lightning Strike</span> $7-10=-3$.</li></ul>
