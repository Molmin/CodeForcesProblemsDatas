## Description

<div><p>You are a usual chat user on the most famous streaming platform. Of course, there are some moments when you just want to chill and spam something.</p><p>More precisely, you want to spam the emote triangle of size $k$. It consists of $2k-1$ messages. The first message consists of one emote, the second one — of two emotes, ..., the $k$-th one — of $k$ emotes, the $k+1$-th one — of $k-1$ emotes, ..., and the last one — of one emote.</p><p>For example, the emote triangle for $k=3$ consists of $5$ messages:</p><center> <img class="tex-graphics" src="file://lSDh9uBu.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Of course, most of the channels have auto moderation. Auto moderator of the current chat will ban you right after you spam at least $x$ emotes in succession (you can assume you are the only user in the chat). Now you are interested — how many messages will you write before getting banned? Or maybe you will not get banned at all (i.e. will write all $2k-1$ messages and complete your emote triangle successfully)? Note that if you get banned as a result of writing a message, this message is also counted.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The next $t$ lines describe test cases.</p><p>The only line of the test case contains integers $k$ and $x$ ($1 \le k \le 10^9; 1 \le x \le 10^{18}$).</p></div><div class="output-specification"><p>For each test case, print the number of messages you will write before getting banned for the corresponding values $k$ and $x$.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The next $t$ lines describe test cases.</p><p>The only line of the test case contains integers $k$ and $x$ ($1 \le k \le 10^9; 1 \le x \le 10^{18}$).</p>

## Output

<p>For each test case, print the number of messages you will write before getting banned for the corresponding values $k$ and $x$.</p>





```input1
7
4 6
4 7
1 2
3 7
2 5
100 1
1000000000 923456789987654321
```




```output1
3
4
1
4
3
1
1608737403
```



## Note

<p>Let's analyze the test cases of the example.</p><ol> <li> In the first test case, you write three messages containing $1$, $2$ and $3$ emotes respectively, and since $1 + 2 + 3 \ge 6$, you get banned after that. </li><li> In the second test case, you write four messages containing $1$, $2$, $3$ and $4$ emotes respectively, and since $1 + 2 + 3 + 4 \ge 7$, you get banned after that. </li><li> In the third test case, you write one message containing exactly $1$ emote. It doesn't get you banned, since $1 &lt; 2$, but you have already finished posting your emote triangle. So you wrote one message successfully. </li><li> In the fourth test case, you write four messages containing $1$, $2$, $3$ and $2$ emotes respectively, and since $1 + 2 + 3 + 2 \ge 7$, you get banned after that. </li><li> In the fifth test case, you write three messages containing $1$, $2$ and $1$ emote respectively. It doesn't get you banned, since $1 + 2 + 1 &lt; 5$, but you have already finished posting your emote triangle. So you wrote three messages successfully. </li><li> In the sixth test case, since $x = 1$, you get banned as soon as you send your first message. </li><li> The seventh test case is too large to analyze, so we'll skip it. </li></ol>
