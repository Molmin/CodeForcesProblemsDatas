## Description

<div><p>Kostya and Zhenya — the creators of the band "Paper" — after the release of the legendary album decided to create a new band "Day movers", for this they need to find two new people.</p><p>They invited $n$ people to the casting. The casting will last $q$ days. On the $i$th of the days, Kostya and Zhenya want to find two people on the segment from $l_i$ to $r_i$ who are most suitable for their band. Since "Day movers" are doing a modern art, musical skills are not important to them and they look only at other signs: they want the height difference between two people to be as small as possible.</p><p>Help them, and for each day, find the minimum difference in the growth of people from the casting on this segment!</p></div><div class="input-specification"><p>In the first line you are given two integers $n$ and $q$ ($2 \leq n \leq 3 \cdot 10^5, 1 \leq q \leq 10^6$)&nbsp;— the number of people who came to the casting and the number of casting days.</p><p>In the second line, you are given $n$ integers $a_1, a_2, a_3, \ldots, a_n$ ($1 \leq a_i \leq n$) — the growth of each of the candidates.</p><p>It is also guaranteed that all $a_i$ <span class="tex-font-style-bf">are different</span>.</p><p>The following $q$ lines each contains two integers $l_i$ and $r_i$ ($1 \leq l_i &lt; r_i \leq n$)&nbsp;— a segment of people on the $i$th day of casting.</p></div><div class="output-specification"><p>Output $q$ lines. In the $i$-th line there should be a minimum height difference between the two candidates on the segment on the $i$-th day of casting.</p></div>

## Input

<p>In the first line you are given two integers $n$ and $q$ ($2 \leq n \leq 3 \cdot 10^5, 1 \leq q \leq 10^6$)&nbsp;— the number of people who came to the casting and the number of casting days.</p><p>In the second line, you are given $n$ integers $a_1, a_2, a_3, \ldots, a_n$ ($1 \leq a_i \leq n$) — the growth of each of the candidates.</p><p>It is also guaranteed that all $a_i$ <span class="tex-font-style-bf">are different</span>.</p><p>The following $q$ lines each contains two integers $l_i$ and $r_i$ ($1 \leq l_i &lt; r_i \leq n$)&nbsp;— a segment of people on the $i$th day of casting.</p>

## Output

<p>Output $q$ lines. In the $i$-th line there should be a minimum height difference between the two candidates on the segment on the $i$-th day of casting.</p>





```input1|
3 3
1 3 2
1 2
2 3
1 3
```




```input2|
5 3
4 1 5 3 2
1 2
3 4
2 4
```




```input3|
7 4
2 6 1 7 3 5 4
4 6
1 2
3 6
1 3
```




```output1
2
1
1
```




```output2
3
2
2
```




```output3
2
4
2
1
```



## Note

<p>In the first example, the minimum difference on the segment $[1, 2]$ is $2$, on the segment $[2, 3]$ — $1$, on the segment $[1, 3]$ is also $1$.</p><p>In the third example, the numbers with the minimum difference on the segment $[4, 6]$ are $3$ and $5$ ($5 - 3 = 2$). On the segment $[1, 2]$, the numbers with the minimum difference are $2$ and $6$ ($6 - 2 = 4$). On the segment $[3, 6]$, the numbers with the minimum difference are $1$ and $3$ ($3 - 1 = 2$). On the segment $[1, 3]$, the minimum difference is formed by the numbers $1$ and $2$ ($2 - 1 = 1$).</p>
