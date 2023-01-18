## Description

<div><p>Filled with optimism, Hyunuk will host a conference about how great this new year will be!</p><p>The conference will have $n$ lectures. Hyunuk has two candidate venues $a$ and $b$. For each of the $n$ lectures, the speaker specified two time intervals $[sa_i, ea_i]$ ($sa_i \le ea_i$) and $[sb_i, eb_i]$ ($sb_i \le eb_i$). If the conference is situated in venue $a$, the lecture will be held from $sa_i$ to $ea_i$, and if the conference is situated in venue $b$, the lecture will be held from $sb_i$ to $eb_i$. Hyunuk will choose one of these venues and <span class="tex-font-style-bf">all</span> lectures will be held at that venue.</p><p>Two lectures are said to overlap if they share any point in time in common. Formally, a lecture held in interval $[x, y]$ overlaps with a lecture held in interval $[u, v]$ if and only if $\max(x, u) \le \min(y, v)$.</p><p>We say that a participant can <span class="tex-font-style-it">attend</span> a subset $s$ of the lectures if the lectures in $s$ do not pairwise overlap (i.e. no two lectures overlap). Note that the possibility of attending may depend on whether Hyunuk selected venue $a$ or venue $b$ to hold the conference.</p><p>A subset of lectures $s$ is said to be <span class="tex-font-style-it">venue-sensitive</span> if, for one of the venues, the participant can attend $s$, but for the other venue, the participant cannot attend $s$.</p><p>A venue-sensitive set is problematic for a participant who is interested in attending the lectures in $s$ because the participant cannot be sure whether the lecture times will overlap. Hyunuk will be happy if and only if there are no venue-sensitive sets. Determine whether Hyunuk will be happy.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 100\,000$), the number of lectures held in the conference.</p><p>Each of the next $n$ lines contains four integers $sa_i$, $ea_i$, $sb_i$, $eb_i$ ($1 \le sa_i, ea_i, sb_i, eb_i \le 10^9$, $sa_i \le ea_i, sb_i \le eb_i$).</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if Hyunuk will be happy. Print "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 100\,000$), the number of lectures held in the conference.</p><p>Each of the next $n$ lines contains four integers $sa_i$, $ea_i$, $sb_i$, $eb_i$ ($1 \le sa_i, ea_i, sb_i, eb_i \le 10^9$, $sa_i \le ea_i, sb_i \le eb_i$).</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if Hyunuk will be happy. Print "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
2
1 2 3 6
3 4 7 8
```




```input2
3
1 3 2 4
4 5 6 7
3 4 5 5
```




```input3
6
1 5 2 9
2 4 5 8
3 6 7 11
7 10 12 16
8 11 13 17
9 12 14 18
```




```output1
YES
```




```output2
NO
```




```output3
YES
```



## Note

<p>In second example, lecture set $\{1, 3\}$ is venue-sensitive. Because participant can't attend this lectures in venue $a$, but can attend in venue $b$.</p><p>In first and third example, venue-sensitive set does not exist.</p>
