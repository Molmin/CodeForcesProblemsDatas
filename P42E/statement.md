## Description

<div><p>Baldman is a warp master. He possesses a unique ability — creating wormholes! Given two positions in space, Baldman can make a wormhole which makes it possible to move between them in both directions. Unfortunately, such operation isn't free for Baldman: each created wormhole makes him lose plenty of hair from his head.</p><p>Because of such extraordinary abilities, Baldman has caught the military's attention. He has been charged with a special task. But first things first.</p><p>The military base consists of several underground objects, some of which are connected with bidirectional tunnels. There necessarily exists a path through the tunnel system between each pair of objects. Additionally, exactly two objects are connected with surface. For the purposes of security, a patrol inspects the tunnel system every day: he enters one of the objects which are connected with surface, walks the base passing each tunnel <span class="tex-font-style-bf">at least</span> once and leaves through one of the objects connected with surface. He can enter and leave either through the same object, or through different objects. The military management noticed that the patrol visits some of the tunnels multiple times and decided to optimize the process. Now they are faced with a problem: a system of wormholes needs to be made to allow of a patrolling which passes each tunnel <span class="tex-font-style-bf">exactly</span> once. At the same time a patrol is allowed to pass each wormhole any number of times.</p><p>This is where Baldman comes to operation: he is the one to plan and build the system of the wormholes. Unfortunately for him, because of strict confidentiality the military can't tell him the arrangement of tunnels. Instead, they insist that his system of portals solves the problem for any arrangement of tunnels which satisfies the given condition. Nevertheless, Baldman has some information: he knows which pairs of objects he can potentially connect and how much it would cost him (in hair). Moreover, tomorrow he will be told which objects (exactly two) are connected with surface. Of course, our hero decided not to waste any time and calculate the minimal cost of getting the job done for some pairs of objects (which he finds likely to be the ones connected with surface). Help Baldman!</p></div><div class="input-specification"><p>First line of the input contains a single natural number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100000</span>) — the number of objects on the military base. The second line — one number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200000</span>) — the number of the wormholes Baldman can make. The following <span class="tex-span"><i>m</i></span> lines describe the wormholes: each line contains three integer numbers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, 1 ≤ <i>c</i> ≤ 100000</span>) — the numbers of objects which can be connected and the number of hair Baldman has to spend to make this wormhole.</p><p>The next line contains one natural number <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100000</span>) — the number of queries. Finally, the last <span class="tex-span"><i>q</i></span> lines contain a description of one query each — a pair of numbers of different objects <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). There could be more than one wormhole between a pair of objects.</p></div><div class="output-specification"><p>Your program should output <span class="tex-span"><i>q</i></span> lines, one for each query. The <span class="tex-span"><i>i</i></span>-th line should contain a single integer number — the answer for <span class="tex-span"><i>i</i></span>-th query: the minimum cost (in hair) of a system of wormholes allowing the optimal patrol for any system of tunnels (satisfying the given conditions) if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the two objects connected with surface, or <span class="tex-font-style-tt">"-1"</span> if such system of wormholes cannot be made.</p></div>

## Input

<p>First line of the input contains a single natural number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100000</span>) — the number of objects on the military base. The second line — one number <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200000</span>) — the number of the wormholes Baldman can make. The following <span class="tex-span"><i>m</i></span> lines describe the wormholes: each line contains three integer numbers <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i>, 1 ≤ <i>c</i> ≤ 100000</span>) — the numbers of objects which can be connected and the number of hair Baldman has to spend to make this wormhole.</p><p>The next line contains one natural number <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 100000</span>) — the number of queries. Finally, the last <span class="tex-span"><i>q</i></span> lines contain a description of one query each — a pair of numbers of different objects <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). There could be more than one wormhole between a pair of objects.</p>

## Output

<p>Your program should output <span class="tex-span"><i>q</i></span> lines, one for each query. The <span class="tex-span"><i>i</i></span>-th line should contain a single integer number — the answer for <span class="tex-span"><i>i</i></span>-th query: the minimum cost (in hair) of a system of wormholes allowing the optimal patrol for any system of tunnels (satisfying the given conditions) if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are the two objects connected with surface, or <span class="tex-font-style-tt">"-1"</span> if such system of wormholes cannot be made.</p>





```input1
2
1
1 2 3
1
1 2

```




```input2
3
1
1 2 3
2
1 2
1 3

```




```output1
0

```




```output2
-1
3

```


