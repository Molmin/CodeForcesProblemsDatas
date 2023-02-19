## Description

<div><p>Once upon a time, in the <span class="tex-font-style-it">Land of the Shamans</span>, everyone lived on the <span class="tex-font-style-it">Sky-High Beanstalk</span>. Each shaman had a unique identifying number $i$ between $0$ and $N-1$, and an altitude value&nbsp;$H_i$, representing how high he lived above ground level. The distance between two altitudes is the absolute value of their difference.</p><p>All shamans lived together in peace, until one of them stole the formula of the world-famous <span class="tex-font-style-it">Potion&nbsp;of&nbsp;Great&nbsp;Power</span>. To cover his/her tracks, the <span class="tex-font-style-it">Thief</span> has put a <span class="tex-font-style-it">Curse</span> on the land: most inhabitants could no longer trust each other...</p><p>Despite the very difficult circumstances, the <span class="tex-font-style-it">Order of Good Investigators</span> have gained the following information about the <span class="tex-font-style-it">Curse</span>: </p><ul>  <li> When the <span class="tex-font-style-it">Curse</span> first takes effect, everyone stops trusting each other.  </li><li> The <span class="tex-font-style-it">Curse</span> is unstable: at the end of each day (exactly at midnight), one pair of shamans will start or stop trusting each other.  </li><li> Unfortunately, each shaman will only ever trust at most $D$ others at any given time. </li></ul> They have also reconstructed a log of who trusted whom: for each night they know which pair of shamans started/stopped trusting each other.<p>They believe the <span class="tex-font-style-it">Thief</span> has whispered the formula to an <span class="tex-font-style-it">Evil Shaman</span>. To avoid detection, both of them visited the home of one of their (respective) trusted friends. During the visit, the <span class="tex-font-style-it">Thief</span> whispered the formula to the <span class="tex-font-style-it">Evil Shaman</span> through the window. (Note: this trusted friend did not have to be home at the time. In fact, it's even possible that they visited each other's houses – shamans are weird.)</p><p>Fortunately, whispers only travel short distances, so the <span class="tex-font-style-it">Order</span> knows the two trusted friends visited (by the <span class="tex-font-style-it">Thief</span> and the <span class="tex-font-style-it">Evil Shaman</span>) must live very close to each other.</p><p>They ask you to help with their investigation. They would like to test their suspicions: what if the <span class="tex-font-style-it">Thief</span> was $x$, the <span class="tex-font-style-it">Evil Shaman</span> was $y$, and the formula was whispered on day $v$? What is the smallest distance the whispered formula had to travel? That is, what is the minimum distance between the apartments of some shamans $x'$ and $y'$ (i.e. $\min\left(\left|H_{x'} - H_{y'}\right|\right)$), such that $x'$ was a trusted friend of $x$ and $y'$ was a trusted friend of $y$ on day&nbsp;$v$?</p><p>They will share all their information with you, then ask you a number of questions. You need to answer each question immediately, before receiving the next one.</p></div><div><h2>Interaction</h2><p>The interaction will begin with a line containing $N$, $D$, $U$ and $Q$ $(2 \leq N \leq 100000$, $1 \leq D \leq 500$, $0 \leq U \leq 200000$, $1 \leq Q \leq 50000)$ – the number of shamans, the maximum number of trusted friends a shaman can have at any given point, the number of days, and the number of questions.</p><p>On the next line $N$ space separated integers will follow, the $i$th $(1\leq i \leq N)$ of which being $H_{i-1}$ $(0\leq H_{i-1} \leq 10^9)$, the altitude of shaman $i-1$.</p><p>On the next $U$ lines there will be two integers each, on the $i$th ($1 \leq i \leq U$) $A_i$ and $B_i$ $(0 \leq A_i, B_i &lt; N$ and $A_i \neq B_i)$, which represents a pair of shamans who started or stopped trusting each other at the end of day $i-1$. That is, if $A_i$ and $B_i$ trusted each other on day $i-1$, they did not trust each other on day $i$, or vice versa. Read all of these integers.</p><p>The interactor now will ask you $Q$ question, so the following interaction should happen $Q$ times: </p><ol> <li> Read $3$ integers describing the current query: $x,y$ and $v$ ($x \neq y$, $0 \leq x,y &lt; N$ and $0 \leq v \leq U$), where $x$ is the suspected <span class="tex-font-style-it">Thief</span>, $y$ is the suspected <span class="tex-font-style-it">Evil Shaman</span>, and $v$ is the suspected day.. </li><li> Then print the answer to this query on a single line, i.e. you should print the minimum distance the whispered formula had to travel from some trusted friend $x'$ of $x$ to a trusted friend $y'$ of $y$. <ul>   <li> <span class="tex-font-style-it">In case someone trusted both $x$ and $y$ (i.e. $x'=y'$), you should print $0$.</span>    </li><li> <span class="tex-font-style-it">If $x$ or $y$ had no trusted friends, print $10^9$.</span> </li></ul> </li></ol><p>After printing each line do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul></div><div><h2>Scoring</h2><center> $ \begin{array}{|c|c|c|} \hline \text{Subtask} &amp; \text{Points} &amp; \text{Constraints} \\ \hline 1 &amp; 0 &amp; \text{samples}\\ \hline 2 &amp; 17 &amp; Q,U \leq 1000 \\ \hline 3 &amp; 14 &amp; v=U \: \text{for all questions} \\ \hline 4 &amp; 18 &amp; H_i \in \left\{0,1\right\} \: \text{for all shamans} \: i \\ \hline 5 &amp; 21 &amp; U,N \leq 10000\\ \hline 6 &amp; 30 &amp; \text{no additional constraints}\\ \hline \end{array} $ </center></div>





```input1
6 5 11 4
2 42 1000 54 68 234
0 1
2 0
3 4
3 5
3 5
1 3
5 3
0 5
3 0
1 3
3 5
0 3 4
3 0 8
0 5 5
3 0 11
```




```output1
26
0
1000000000
14
```



## Note

<p>Example queries: <img class="tex-graphics" src="file://qi9eNIBl.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Evolution of friendships: <img class="tex-graphics" src="file://eQHVj0l1.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
