## Description

<div><p>Mishka's favourite experimental indie band has recently dropped a new album! Songs of that album share one gimmick. Each name $s_i$ is one of the following types:</p><ul> <li> $1~c$ — a single lowercase Latin letter; </li><li> $2~j~c$ — name $s_j$ ($1 \le j &lt; i$) with a single lowercase Latin letter appended to its end. </li></ul><p>Songs are numbered from $1$ to $n$. It's guaranteed that the first song is always of type $1$.</p><p>Vova is rather interested in the new album but he really doesn't have the time to listen to it entirely. Thus he asks Mishka some questions about it to determine if some song is worth listening to. Questions have the following format:</p><ul> <li> $i~t$ — count the number of occurrences of string $t$ in $s_i$ (the name of the $i$-th song of the album) as a continuous substring, $t$ consists only of lowercase Latin letters. </li></ul><p>Mishka doesn't question the purpose of that information, yet he struggles to provide it. Can you please help Mishka answer all Vova's questions?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 4 \cdot 10^5$) — the number of songs in the album.</p><p>Each of the next $n$ lines contains the desciption of the $i$-th song of the album in the following format:</p><ul> <li> $1~c$ — $s_i$ is a single lowercase Latin letter; </li><li> $2~j~c$ — $s_i$ is the name $s_j$ ($1 \le j &lt; i$) with a single lowercase Latin letter appended to its end. </li></ul><p>The next line contains a single integer $m$ ($1 \le m \le 4 \cdot 10^5$) — the number of Vova's questions.</p><p>Each of the next $m$ lines contains the desciption of the $j$-th Vova's question in the following format:</p><ul> <li> $i~t$ ($1 \le i \le n$, $1 \le |t| \le 4 \cdot 10^5$) — count the number of occurrences of string $t$ in $s_i$ (the name of the $i$-th song of the album) as a continuous substring, $t$ consists only of lowercase Latin letters. </li></ul><p><span class="tex-font-style-bf">It's guaranteed that the total length of question strings $t$ doesn't exceed $4 \cdot 10^5$</span>.</p></div><div class="output-specification"><p>For each question print a single integer — the number of occurrences of the question string $t$ in the name of the $i$-th song of the album as a continuous substring.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 4 \cdot 10^5$) — the number of songs in the album.</p><p>Each of the next $n$ lines contains the desciption of the $i$-th song of the album in the following format:</p><ul> <li> $1~c$ — $s_i$ is a single lowercase Latin letter; </li><li> $2~j~c$ — $s_i$ is the name $s_j$ ($1 \le j &lt; i$) with a single lowercase Latin letter appended to its end. </li></ul><p>The next line contains a single integer $m$ ($1 \le m \le 4 \cdot 10^5$) — the number of Vova's questions.</p><p>Each of the next $m$ lines contains the desciption of the $j$-th Vova's question in the following format:</p><ul> <li> $i~t$ ($1 \le i \le n$, $1 \le |t| \le 4 \cdot 10^5$) — count the number of occurrences of string $t$ in $s_i$ (the name of the $i$-th song of the album) as a continuous substring, $t$ consists only of lowercase Latin letters. </li></ul><p><span class="tex-font-style-bf">It's guaranteed that the total length of question strings $t$ doesn't exceed $4 \cdot 10^5$</span>.</p>

## Output

<p>For each question print a single integer — the number of occurrences of the question string $t$ in the name of the $i$-th song of the album as a continuous substring.</p>





```input1
20
1 d
2 1 a
2 2 d
2 3 a
2 4 d
2 5 a
2 6 d
2 7 a
1 d
2 9 o
2 10 k
2 11 i
2 12 d
2 13 o
2 14 k
2 15 i
2 1 o
2 17 k
2 18 i
2 15 i
12
8 da
8 dada
8 ada
6 dada
3 dada
19 doki
19 ok
16 doki
15 doki
9 d
1 a
20 doki
```




```output1
4
3
3
2
0
1
1
2
1
1
0
2
```



## Note

<p>Song names of the first example:</p><ol> <li> d </li><li> da </li><li> dad </li><li> dada </li><li> dadad </li><li> dadada </li><li> dadadad </li><li> dadadada </li><li> d </li><li> do </li><li> dok </li><li> doki </li><li> dokid </li><li> dokido </li><li> dokidok </li><li> dokidoki </li><li> do </li><li> dok </li><li> doki </li><li> dokidoki </li></ol><p>Thus the occurrences for each question string are:</p><ol> <li> string "da" starts in positions $[1, 3, 5, 7]$ in the name "dadadada"; </li><li> string "dada" starts in positions $[1, 3, 5]$ in the name "dadadada"; </li><li> string "ada" starts in positions $[2, 4, 6]$ in the name "dadadada"; </li><li> string "dada" starts in positions $[1, 3]$ in the name "dadada"; </li><li> no occurrences of string "dada" in the name "dad"; </li><li> string "doki" starts in position $[1]$ in the name "doki"; </li><li> string "ok" starts in position $[2]$ in the name "doki"; </li><li> string "doki" starts in positions $[1, 5]$ in the name "dokidoki"; </li><li> string "doki" starts in position $[1]$ in the name "dokidok"; </li><li> string "d" starts in position $[1]$ in the name "d"; </li><li> no occurrences of string "a" in the name "d"; </li><li> string "doki" starts in positions $[1, 5]$ in the name "dokidoki". </li></ol>
