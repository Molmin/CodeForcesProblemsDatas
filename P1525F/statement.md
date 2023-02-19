## Description

<div><p>Monocarp plays a computer game called "Goblins and Gnomes". In this game, he manages a large underground city of gnomes and defends it from hordes of goblins.</p><p>The city consists of $n$ halls and $m$ one-directional tunnels connecting them. The structure of tunnels has the following property: if a goblin leaves any hall, he cannot return to that hall. </p><p>The city will be attacked by $k$ waves of goblins; during the $i$-th wave, $i$ goblins attack the city. Monocarp's goal is to pass all $k$ waves.</p><p>The $i$-th wave goes as follows: firstly, $i$ goblins appear in some halls of the city and pillage them; <span class="tex-font-style-bf">at most one goblin appears in each hall</span>. Then, goblins start moving along the tunnels, pillaging all the halls in their path. </p><p>Goblins are very greedy and cunning, so they choose their paths so that no two goblins pass through the same hall. Among all possible attack plans, they choose a plan which allows them to <span class="tex-font-style-bf">pillage the maximum number of halls</span>. After goblins are done pillaging, they leave the city.</p><p>If all halls are pillaged during the wave — Monocarp loses the game. Otherwise, the city is restored. If some hall is pillaged during a wave, goblins are still interested in pillaging it during the next waves.</p><p>Before each wave, Monocarp can spend some time preparing to it. Monocarp doesn't have any strict time limits on his preparations (he decides when to call each wave by himself), but the longer he prepares for a wave, the fewer points he gets for passing it. If Monocarp prepares for the $i$-th wave for $t_i$ minutes, then he gets $\max(0, x_i - t_i \cdot y_i)$ points for passing it (obviously, if he doesn't lose in the process).</p><p>While preparing for a wave, Monocarp can block tunnels. He can spend one minute to <span class="tex-font-style-bf">either block all tunnels leading from some hall or block all tunnels leading to some hall</span>. If Monocarp blocks a tunnel while preparing for a wave, it stays blocked during the next waves as well.</p><p>Help Monocarp to defend against all $k$ waves of goblins and get the maximum possible amount of points!</p></div><div class="input-specification"><p>The first line contains three integers $n$, $m$ and $k$ ($2 \le n \le 50$; $0 \le m \le \frac{n(n - 1)}{2}$; $1 \le k \le n - 1$)&nbsp;— the number of halls in the city, the number of tunnels and the number of goblin waves, correspondely.</p><p>Next $m$ lines describe tunnels. The $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$; $u_i \ne v_i$). It means that the tunnel goes from hall $u_i$ to hall $v_i$. <span class="tex-font-style-bf">The structure of tunnels has the following property: if a goblin leaves any hall, he cannot return to that hall</span>. There is at most one tunnel between each pair of halls.</p><p>Next $k$ lines describe the scoring system. The $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i \le 10^9$; $1 \le y_i \le 10^9$). If Monocarp prepares for the $i$-th wave for $t_i$ minutes, then he gets $\max(0, x_i - t_i \cdot y_i)$ points for passing it.</p></div><div class="output-specification"><p>Print the optimal Monocarp's strategy in the following format:</p><p>At first, print one integer $a$ ($k \le a \le 2n + k$)&nbsp;— the number of actions Monocarp will perform. Next, print actions themselves in the order Monocarp performs them. The $i$-th action is described by a single integer $b_i$ ($-n \le b_i \le n$) using the following format:</p><ul> <li> if $b_i &gt; 0$ then Monocarp blocks all tunnels going out from the hall $b_i$; </li><li> if $b_i &lt; 0$ then Monocarp blocks all tunnels going into the hall $|b_i|$; </li><li> if $b_i = 0$ then Monocarp calls the next goblin wave. </li></ul><p>You can't repeat the same block action $b_i$ several times. Monocarp must survive all waves he calls (goblins shouldn't be able to pillage all halls). Monocarp should call exactly $k$ waves and earn the maximum possible number of points in total.</p><p>If there are several optimal strategies&nbsp;— print any of them.</p></div>

## Input

<p>The first line contains three integers $n$, $m$ and $k$ ($2 \le n \le 50$; $0 \le m \le \frac{n(n - 1)}{2}$; $1 \le k \le n - 1$)&nbsp;— the number of halls in the city, the number of tunnels and the number of goblin waves, correspondely.</p><p>Next $m$ lines describe tunnels. The $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$; $u_i \ne v_i$). It means that the tunnel goes from hall $u_i$ to hall $v_i$. <span class="tex-font-style-bf">The structure of tunnels has the following property: if a goblin leaves any hall, he cannot return to that hall</span>. There is at most one tunnel between each pair of halls.</p><p>Next $k$ lines describe the scoring system. The $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i \le 10^9$; $1 \le y_i \le 10^9$). If Monocarp prepares for the $i$-th wave for $t_i$ minutes, then he gets $\max(0, x_i - t_i \cdot y_i)$ points for passing it.</p>

## Output

<p>Print the optimal Monocarp's strategy in the following format:</p><p>At first, print one integer $a$ ($k \le a \le 2n + k$)&nbsp;— the number of actions Monocarp will perform. Next, print actions themselves in the order Monocarp performs them. The $i$-th action is described by a single integer $b_i$ ($-n \le b_i \le n$) using the following format:</p><ul> <li> if $b_i &gt; 0$ then Monocarp blocks all tunnels going out from the hall $b_i$; </li><li> if $b_i &lt; 0$ then Monocarp blocks all tunnels going into the hall $|b_i|$; </li><li> if $b_i = 0$ then Monocarp calls the next goblin wave. </li></ul><p>You can't repeat the same block action $b_i$ several times. Monocarp must survive all waves he calls (goblins shouldn't be able to pillage all halls). Monocarp should call exactly $k$ waves and earn the maximum possible number of points in total.</p><p>If there are several optimal strategies&nbsp;— print any of them.</p>





```input1
5 4 4
1 2
2 3
4 3
5 3
100 1
200 5
10 10
100 1
```




```input2
5 4 4
1 2
2 3
4 3
5 3
100 100
200 5
10 10
100 1
```




```input3
5 10 1
1 2
1 3
1 4
1 5
5 2
5 3
5 4
4 2
4 3
2 3
100 100
```




```output1
6
-2 -3 0 0 0 0
```




```output2
6
0 -3 0 0 1 0
```




```output3
6
1 2 3 4 5 0
```



## Note

<p>In the first example, Monocarp, firstly, block all tunnels going in hall $2$, secondly&nbsp;— all tunnels going in hall $3$, and after that calls all waves. He spent two minutes to prepare to wave $1$, so he gets $98$ points for it. He didn't prepare after that, that's why he gets maximum scores for each of next waves ($200$, $10$ and $100$). In total, Monocarp earns $408$ points.</p><p>In the second example, Monocarp calls for the first wave immediately and gets $100$ points. Before the second wave he blocks all tunnels going in hall $3$. He spent one minute preparing to the wave, so he gets $195$ points. Monocarp didn't prepare for the third wave, so he gets $10$ points by surviving it. Before the fourth wave he blocks all tunnels going out from hall $1$. He spent one minute, so he gets $99$ points for the fourth wave. In total, Monocarp earns $404$ points.</p><p>In the third example, it doesn't matter how many minutes Monocarp will spend before the wave, since he won't get any points for it. That's why he decides to block all tunnels in the city, spending $5$ minutes. He survived the wave though without getting any points.</p>
