## Description

<div><p>Your friend is developing a computer game. He has already decided how the game world should look like — it should consist of $n$ locations connected by $m$ <span class="tex-font-style-bf">two-way</span> passages. The passages are designed in such a way that it should be possible to get from any location to any other location.</p><p>Of course, some passages should be guarded by the monsters (if you just can go everywhere without any difficulties, then it's not fun, right?). Some crucial passages will be guarded by really fearsome monsters, requiring the hero to prepare for battle and designing his own tactics of defeating them (commonly these kinds of monsters are called <span class="tex-font-style-bf">bosses</span>). And your friend wants you to help him place these bosses.</p><p>The game will start in location $s$ and end in location $t$, but these locations are not chosen yet. After choosing these locations, your friend will place a boss in each passage such that it is impossible to get from $s$ to $t$ without using this passage. Your friend wants to place as much bosses as possible (because more challenges means more fun, right?), so he asks you to help him determine the maximum possible number of bosses, considering that any location can be chosen as $s$ or as $t$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 3 \cdot 10^5$, $n - 1 \le m \le 3 \cdot 10^5$) — the number of locations and passages, respectively.</p><p>Then $m$ lines follow, each containing two integers $x$ and $y$ ($1 \le x, y \le n$, $x \ne y$) describing the endpoints of one of the passages.</p><p>It is guaranteed that there is no pair of locations directly connected by two or more passages, and that any location is reachable from any other location.</p></div><div class="output-specification"><p>Print one integer — the maximum number of bosses your friend can place, considering all possible choices for $s$ and $t$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 3 \cdot 10^5$, $n - 1 \le m \le 3 \cdot 10^5$) — the number of locations and passages, respectively.</p><p>Then $m$ lines follow, each containing two integers $x$ and $y$ ($1 \le x, y \le n$, $x \ne y$) describing the endpoints of one of the passages.</p><p>It is guaranteed that there is no pair of locations directly connected by two or more passages, and that any location is reachable from any other location.</p>

## Output

<p>Print one integer — the maximum number of bosses your friend can place, considering all possible choices for $s$ and $t$.</p>





```input1
5 5
1 2
2 3
3 1
4 1
5 2

```




```input2
4 3
1 2
4 3
3 2

```




```output1
2

```




```output2
3

```


