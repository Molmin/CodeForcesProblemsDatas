## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">Don't you tell me what you think that I can be</span></div></div><p>If you say that Arkady is a bit old-fashioned playing checkers, you won't be right. There is also a modern computer game Arkady and his friends are keen on. We won't discuss its rules, the only feature important to this problem is that each player has to pick a distinct hero in the beginning of the game.</p><p>There are $2$ teams each having $n$ players and $2n$ heroes to distribute between the teams. The teams take turns picking heroes: at first, the first team chooses a hero in its team, after that the second team chooses a hero and so on. Note that after a hero is chosen it becomes unavailable to both teams.</p><p>The friends estimate the power of the $i$-th of the heroes as $p_i$. Each team wants to maximize the total power of its heroes. However, there is one exception: there are $m$ pairs of heroes that are especially strong against each other, so when any team chooses a hero from such a pair, the other team <span class="tex-font-style-bf">must</span> choose the other one on its turn. Each hero is in at most one such pair.</p><p>This is an interactive problem. You are to write a program that will optimally choose the heroes for one team, while the jury's program will play for the other team. Note that the jury's program may behave inefficiently, in this case you have to take the opportunity and still maximize the total power of your team. Formally, if you ever have chance to reach the total power of $q$ or greater regardless of jury's program choices, you must get $q$ or greater to pass a test.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^3$, $0 \le m \le n$)&nbsp;— the number of players in one team and the number of special pairs of heroes.</p><p>The second line contains $2n$ integers $p_1, p_2, \ldots, p_{2n}$ ($1 \le p_i \le 10^3$)&nbsp;— the powers of the heroes.</p><p>Each of the next $m$ lines contains two integer $a$ and $b$ ($1 \le a, b \le 2n$, $a \ne b$)&nbsp;— a pair of heroes that are especially strong against each other. It is guaranteed that each hero appears at most once in this list.</p><p>The next line contains a single integer $t$ ($1 \le t \le 2$)&nbsp;— the team you are to play for. If $t = 1$, the first turn is yours, otherwise you have the second turn.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>In order to hack, use the format described above with one additional line. In this line output $2n$ distinct integers from $1$ to $2n$&nbsp;— the priority order for the jury's team. The jury's team will on each turn select the first possible hero from this list. Here possible means that it is not yet taken and does not contradict the rules about special pair of heroes.</p></div><div><h2>Interaction</h2><p>When it is your turn, print a single integer $x$ ($1 \le x \le 2n$)&nbsp;— the index of the hero chosen by you. Note that you can't choose a hero previously chosen by either you of the other player, and you must follow the rules about special pairs of heroes.</p><p>When it is the other team's turn, read a line containing a single integer $x$ ($1 \le x \le 2n$)&nbsp;— the index of the hero chosen by the other team. It is guaranteed that this index is not chosen before and that the other team also follows the rules about special pairs of heroes.</p><p>After the last turn you should terminate without printing anything.</p><p>After printing your choice do not forget to output end of line and flush the output. Otherwise you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p>Jury's answer $-1$ instead of a valid choice means that you made an invalid turn. Exit immediately after receiving $-1$ and you will see <span class="tex-font-style-tt">Wrong answer</span> verdict. Otherwise you can get an arbitrary verdict because your solution will continue to read from a closed stream.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^3$, $0 \le m \le n$)&nbsp;— the number of players in one team and the number of special pairs of heroes.</p><p>The second line contains $2n$ integers $p_1, p_2, \ldots, p_{2n}$ ($1 \le p_i \le 10^3$)&nbsp;— the powers of the heroes.</p><p>Each of the next $m$ lines contains two integer $a$ and $b$ ($1 \le a, b \le 2n$, $a \ne b$)&nbsp;— a pair of heroes that are especially strong against each other. It is guaranteed that each hero appears at most once in this list.</p><p>The next line contains a single integer $t$ ($1 \le t \le 2$)&nbsp;— the team you are to play for. If $t = 1$, the first turn is yours, otherwise you have the second turn.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>In order to hack, use the format described above with one additional line. In this line output $2n$ distinct integers from $1$ to $2n$&nbsp;— the priority order for the jury's team. The jury's team will on each turn select the first possible hero from this list. Here possible means that it is not yet taken and does not contradict the rules about special pair of heroes.</p>





```input1
3 1
1 2 3 4 5 6
2 6
1

2

4

1
```




```input2
3 1
1 2 3 4 5 6
1 5
2
6

1

3
```




```output1
6

5

3
```




```output2
5

4

2
```



## Note

<p>In the first example the first turn is yours. In example, you choose $6$, the other team is forced to reply with $2$. You choose $5$, the other team chooses $4$. Finally, you choose $3$ and the other team choose $1$.</p><p>In the second example you have the second turn. The other team chooses $6$, you choose $5$, forcing the other team to choose $1$. Now you choose $4$, the other team chooses $3$ and you choose $2$.</p>
