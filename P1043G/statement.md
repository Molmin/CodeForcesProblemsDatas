## Description

<div><p>Ildar took a band (a thin strip of cloth) and colored it. Formally, the band has $n$ cells, each of them is colored into one of $26$ colors, so we can denote each color with one of the lowercase letters of English alphabet. </p><p>Ildar decided to take some segment of the band $[l, r]$ ($1 \le l \le r \le n$) he likes and cut it from the band. So he will create a new band that can be represented as a string $t = s_l s_{l+1} \ldots s_r$.</p><p>After that Ildar will play the following game: he cuts the band $t$ into some new bands and counts the number of different bands among them. Formally, Ildar chooses $1 \le k \le |t|$ indexes $1 \le i_1 &lt; i_2 &lt; \ldots &lt; i_k = |t|$ and cuts $t$ to $k$ bands-strings $t_1 t_2 \ldots t_{i_1}, t_{i_1 + 1} \ldots t_{i_2}, \ldots, {t_{i_{k-1} + 1}} \ldots t_{i_k}$ and counts the number of different bands among them. He wants to know the minimal possible number of different bands he can get under the constraint that at least one band repeats at least two times. The result of the game is this number. If it is impossible to cut $t$ in such a way, the result of the game is <span class="tex-font-style-tt">-1</span>.</p><p>Unfortunately Ildar hasn't yet decided which segment he likes, but he has $q$ segments-candidates $[l_1, r_1]$, $[l_2, r_2]$, ..., $[l_q, r_q]$. Your task is to calculate the result of the game for each of them.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the length of the band Ildar has.</p><p>The second line contains a string $s$ consisting of $n$ lowercase English letters&nbsp;— the band Ildar has.</p><p>The third line contains a single integer $q$ ($1 \le q \le 200\,000$)&nbsp;— the number of segments Ildar has chosen as candidates.</p><p>Each of the next $q$ lines contains two integer integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) denoting the ends of the $i$-th segment.</p></div><div class="output-specification"><p>Output $q$ lines, where the $i$-th of them should contain the result of the game on the segment $[l_i, r_i]$.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 200\,000$)&nbsp;— the length of the band Ildar has.</p><p>The second line contains a string $s$ consisting of $n$ lowercase English letters&nbsp;— the band Ildar has.</p><p>The third line contains a single integer $q$ ($1 \le q \le 200\,000$)&nbsp;— the number of segments Ildar has chosen as candidates.</p><p>Each of the next $q$ lines contains two integer integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$) denoting the ends of the $i$-th segment.</p>

## Output

<p>Output $q$ lines, where the $i$-th of them should contain the result of the game on the segment $[l_i, r_i]$.</p>





```input1
9
abcabcdce
7
1 6
4 7
5 9
6 9
1 9
3 6
4 4

```




```output1
1
-1
4
3
2
2
-1

```



## Note

<p>Consider the first example.</p><p>If Ildar chooses the segment $[1, 6]$, he cuts a string $t = abcabc$. If he cuts $t$ into two bands $abc$ and $abc$, the band $abc$ repeats two times and the number of different tapes is $1$. So, the result of this game is $1$.</p><p>If Ildar chooses the segment $[4, 7]$, he cuts a string $t = abcd$. It is impossible to cut this band in such a way that there is at least one band repeating at least two times. So, the result of this game is $-1$.</p><p>If Ildar chooses the segment $[3, 6]$, he cuts a string $t = cabc$. If he cuts $t$ into three bands $c$, $ab$ and $c$, the band $c$ repeats two times and the number of different bands is $2$. So, the result of this game is $2$.</p>
