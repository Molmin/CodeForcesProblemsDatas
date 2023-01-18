## Description

<div><p>The Berland Forest can be represented as an infinite cell plane. Every cell contains a tree. That is, contained before the recent events.</p><p>A destructive fire raged through the Forest, and several trees were damaged by it. Precisely speaking, you have a $n \times m$ rectangle map which represents the damaged part of the Forest. The damaged trees were marked as "<span class="tex-font-style-tt">X</span>" while the remaining ones were marked as "<span class="tex-font-style-tt">.</span>". <span class="tex-font-style-bf">You are sure that all burnt trees are shown on the map. All the trees outside the map are undamaged.</span></p><p>The firemen quickly extinguished the fire, and now they are investigating the cause of it. The main version is that there was an arson: at some moment of time (let's consider it as $0$) some trees were set on fire. At the beginning of minute $0$, only the trees that were set on fire initially were burning. At the end of each minute, the fire spread from every burning tree to each of $8$ neighboring trees. At the beginning of minute $T$, the fire was extinguished.</p><p>The firemen want to find the arsonists as quickly as possible. The problem is, they know neither the value of $T$ (how long the fire has been raging) nor the coordinates of the trees that were initially set on fire. They want you to find the maximum value of $T$ (to know how far could the arsonists escape) and a possible set of trees that could be initially set on fire.</p><p>Note that you'd like to maximize value $T$ but the set of trees can be arbitrary.</p></div><div class="input-specification"><p>The first line contains two integer $n$ and $m$ ($1 \le n, m \le 10^6$, $1 \le n \cdot m \le 10^6$) — the sizes of the map.</p><p>Next $n$ lines contain the map. The $i$-th line corresponds to the $i$-th row of the map and contains $m$-character string. The $j$-th character of the $i$-th string is "<span class="tex-font-style-tt">X</span>" if the corresponding tree is burnt and "<span class="tex-font-style-tt">.</span>" otherwise.</p><p>It's guaranteed that the map contains at least one "<span class="tex-font-style-tt">X</span>".</p></div><div class="output-specification"><p>In the first line print the single integer $T$ — the maximum time the Forest was on fire. In the next $n$ lines print the certificate: the map ($n \times m$ rectangle) where the trees that were set on fire are marked as "<span class="tex-font-style-tt">X</span>" and all other trees are marked as "<span class="tex-font-style-tt">.</span>".</p></div>

## Input

<p>The first line contains two integer $n$ and $m$ ($1 \le n, m \le 10^6$, $1 \le n \cdot m \le 10^6$) — the sizes of the map.</p><p>Next $n$ lines contain the map. The $i$-th line corresponds to the $i$-th row of the map and contains $m$-character string. The $j$-th character of the $i$-th string is "<span class="tex-font-style-tt">X</span>" if the corresponding tree is burnt and "<span class="tex-font-style-tt">.</span>" otherwise.</p><p>It's guaranteed that the map contains at least one "<span class="tex-font-style-tt">X</span>".</p>

## Output

<p>In the first line print the single integer $T$ — the maximum time the Forest was on fire. In the next $n$ lines print the certificate: the map ($n \times m$ rectangle) where the trees that were set on fire are marked as "<span class="tex-font-style-tt">X</span>" and all other trees are marked as "<span class="tex-font-style-tt">.</span>".</p>





```input1
3 6
XXXXXX
XXXXXX
XXXXXX
```




```input2
10 10
.XXXXXX...
.XXXXXX...
.XXXXXX...
.XXXXXX...
.XXXXXXXX.
...XXXXXX.
...XXXXXX.
...XXXXXX.
...XXXXXX.
..........
```




```input3
4 5
X....
..XXX
..XXX
..XXX
```




```output1
1
......
.X.XX.
......
```




```output2
2
..........
..........
...XX.....
..........
..........
..........
.....XX...
..........
..........
..........
```




```output3
0
X....
..XXX
..XXX
..XXX
```


