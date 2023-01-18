## Description

<div><p>As we all know, Eleven has special abilities. Thus, Hopper convinced her to close the gate to the Upside Down World with her mind. Upside down monsters like to move between the worlds, so they are going to attack Hopper and Eleven in order to make them stop. The monsters live in the vines. The vines form a tree with <span class="tex-span"><i>n</i></span> vertices, numbered from <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. There's a lowercase English letter written in each tunnel (edge).</p><center> <img class="tex-graphics" src="file://57BqFq4e.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Upside down is a magical world. There are <span class="tex-span"><i>m</i></span> types of monsters in upside down, numbered from <span class="tex-span">1</span> through <span class="tex-span"><i>m</i></span>. Each type of monster has a special word that gives them powers. The special word of type <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. There are <span class="tex-span"><i>q</i></span> monsters in upside down. Each one is at a junction (vertex) and is going to some other junction. If monster of type <span class="tex-span"><i>k</i></span> goes from junction <span class="tex-span"><i>i</i></span> to junction <span class="tex-span"><i>j</i></span>, the power it gains is the number of times it sees its special world (<span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span>) consecutively in the tunnels. More formally: </p><p>If <span class="tex-span"><i>f</i>(<i>i</i>, <i>j</i>)</span> is the string we get when we concatenate the letters written in the tunnels on the shortest path from <span class="tex-span"><i>i</i></span> to <span class="tex-span"><i>j</i></span>, then the power the monster gains is the number of occurrences of <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub></span> in <span class="tex-span"><i>f</i>(<i>i</i>, <i>j</i>)</span>.</p><p>Hopper and Eleven want to get prepared, so for each monster, they want to know the power the monster gains after moving. </p></div><div class="input-specification"><p>The first line of input contains three integers, <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the tunnels (edges). Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>) and a lowercase English letter <span class="tex-span"><i>c</i></span>, meaning there's a tunnel connecting junctions <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> written <span class="tex-span"><i>c</i></span> in it. It is guaranteed that the given graph is a tree.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the special words. <span class="tex-span"><i>i</i></span>-th line of them contains a single string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>), consisting of lowercase English letters. It is guaranteed that <span class="tex-span">|<i>s</i><sub class="lower-index">1</sub>| + |<i>s</i><sub class="lower-index">2</sub>| + ... + |<i>s</i><sub class="lower-index"><i>m</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the monsters. Each line contains three integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i> ≠ <i>j</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>m</i></span>), meaning a monster of type <span class="tex-span"><i>k</i></span> is going from junction number <span class="tex-span"><i>i</i></span> to junction number <span class="tex-span"><i>j</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. <span class="tex-span"><i>i</i></span>-th line should contain a single integer, the power the <span class="tex-span"><i>i</i></span>-th monster gains after moving.</p></div>

## Input

<p>The first line of input contains three integers, <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain the tunnels (edges). Each line contains two integers <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> (<span class="tex-span">1 ≤ <i>v</i>, <i>u</i> ≤ <i>n</i></span>, <span class="tex-span"><i>v</i> ≠ <i>u</i></span>) and a lowercase English letter <span class="tex-span"><i>c</i></span>, meaning there's a tunnel connecting junctions <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>u</i></span> written <span class="tex-span"><i>c</i></span> in it. It is guaranteed that the given graph is a tree.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the special words. <span class="tex-span"><i>i</i></span>-th line of them contains a single string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>), consisting of lowercase English letters. It is guaranteed that <span class="tex-span">|<i>s</i><sub class="lower-index">1</sub>| + |<i>s</i><sub class="lower-index">2</sub>| + ... + |<i>s</i><sub class="lower-index"><i>m</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the monsters. Each line contains three integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i> ≠ <i>j</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>m</i></span>), meaning a monster of type <span class="tex-span"><i>k</i></span> is going from junction number <span class="tex-span"><i>i</i></span> to junction number <span class="tex-span"><i>j</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. <span class="tex-span"><i>i</i></span>-th line should contain a single integer, the power the <span class="tex-span"><i>i</i></span>-th monster gains after moving.</p>





```input1
6 4 5
1 6 b
2 3 a
1 2 b
5 3 b
4 5 b
a
b
bb
aa
1 2 1
6 2 3
1 6 2
4 5 4
1 6 2

```




```input2
10 6 7
1 3 s
10 1 d
2 6 s
5 2 d
7 4 l
8 9 d
8 10 l
7 2 d
8 7 l
dl
dssld
d
d
l
sl
4 5 4
3 7 5
10 6 2
3 1 4
7 5 6
10 9 4
9 8 4

```




```output1
0
1
1
0
1

```




```output2
2
2
0
0
0
1
1

```


