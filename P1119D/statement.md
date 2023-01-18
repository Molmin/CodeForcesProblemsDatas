## Description

<div><p>Miyako came to the flea kingdom with a ukulele. She became good friends with local flea residents and played beautiful music for them every day.</p><p>In return, the fleas made a bigger ukulele for her: it has $n$ <span class="tex-font-style-it">strings</span>, and each string has $(10^{18} + 1)$ <span class="tex-font-style-it">frets</span> numerated from $0$ to $10^{18}$. The fleas use the array $s_1, s_2, \ldots, s_n$ to describe the ukulele's tuning, that is, the <span class="tex-font-style-it">pitch</span> of the $j$-th fret on the $i$-th string is the integer $s_i + j$.</p><p>Miyako is about to leave the kingdom, but the fleas hope that Miyako will answer some last questions for them.</p><p>Each question is in the form of: "How many different pitches are there, if we consider frets between $l$ and $r$ (inclusive) on all strings?"</p><p>Miyako is about to visit the cricket kingdom and has no time to answer all the questions. Please help her with this task!</p><p>Formally, you are given a matrix with $n$ rows and $(10^{18}+1)$ columns, where the cell in the $i$-th row and $j$-th column ($0 \le j \le 10^{18}$) contains the integer $s_i + j$. You are to answer $q$ queries, in the $k$-th query you have to answer the number of distinct integers in the matrix from the $l_k$-th to the $r_k$-th columns, inclusive.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \leq n \leq 100\,000$)&nbsp;— the number of strings.</p><p>The second line contains $n$ integers $s_1, s_2, \ldots, s_n$ ($0 \leq s_i \leq 10^{18}$)&nbsp;— the tuning of the ukulele.</p><p>The third line contains an integer $q$ ($1 \leq q \leq 100\,000$)&nbsp;— the number of questions.</p><p>The $k$-th among the following $q$ lines contains two integers $l_k$，$r_k$ ($0 \leq l_k \leq r_k \leq 10^{18}$)&nbsp;— a question from the fleas.</p></div><div class="output-specification"><p>Output one number for each question, separated by spaces&nbsp;— the number of different pitches.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \leq n \leq 100\,000$)&nbsp;— the number of strings.</p><p>The second line contains $n$ integers $s_1, s_2, \ldots, s_n$ ($0 \leq s_i \leq 10^{18}$)&nbsp;— the tuning of the ukulele.</p><p>The third line contains an integer $q$ ($1 \leq q \leq 100\,000$)&nbsp;— the number of questions.</p><p>The $k$-th among the following $q$ lines contains two integers $l_k$，$r_k$ ($0 \leq l_k \leq r_k \leq 10^{18}$)&nbsp;— a question from the fleas.</p>

## Output

<p>Output one number for each question, separated by spaces&nbsp;— the number of different pitches.</p>





```input1
6
3 1 4 1 5 9
3
7 7
0 2
8 17

```




```input2
2
1 500000000000000000
2
1000000000000000000 1000000000000000000
0 1000000000000000000

```




```output1
5 10 18

```




```output2
2 1500000000000000000

```



## Note

<p>For the first example, the pitches on the $6$ strings are as follows.</p><p>$$ \begin{matrix} \textbf{Fret} &amp; \textbf{0} &amp; \textbf{1} &amp; \textbf{2} &amp; \textbf{3} &amp; \textbf{4} &amp; \textbf{5} &amp; \textbf{6} &amp; \textbf{7} &amp; \ldots \\ s_1: &amp; 3 &amp; 4 &amp; 5 &amp; 6 &amp; 7 &amp; 8 &amp; 9 &amp; 10 &amp; \dots \\ s_2: &amp; 1 &amp; 2 &amp; 3 &amp; 4 &amp; 5 &amp; 6 &amp; 7 &amp; 8 &amp; \dots \\ s_3: &amp; 4 &amp; 5 &amp; 6 &amp; 7 &amp; 8 &amp; 9 &amp; 10 &amp; 11 &amp; \dots \\ s_4: &amp; 1 &amp; 2 &amp; 3 &amp; 4 &amp; 5 &amp; 6 &amp; 7 &amp; 8 &amp; \dots \\ s_5: &amp; 5 &amp; 6 &amp; 7 &amp; 8 &amp; 9 &amp; 10 &amp; 11 &amp; 12 &amp; \dots \\ s_6: &amp; 9 &amp; 10 &amp; 11 &amp; 12 &amp; 13 &amp; 14 &amp; 15 &amp; 16 &amp; \dots \end{matrix} $$</p><p>There are $5$ different pitches on fret $7$&nbsp;— $8, 10, 11, 12, 16$.</p><p>There are $10$ different pitches on frets $0, 1, 2$&nbsp;— $1, 2, 3, 4, 5, 6, 7, 9, 10, 11$.</p>
