## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is the constraints</span>.</p><p>Polycarp has to write a coursework. The coursework consists of $m$ pages.</p><p>Polycarp also has $n$ cups of coffee. The coffee in the $i$-th cup Polycarp has $a_i$ caffeine in it. Polycarp can drink some cups of coffee (each one no more than once). He can drink cups in <span class="tex-font-style-bf">any order</span>. Polycarp drinks each cup <span class="tex-font-style-bf">instantly</span> and <span class="tex-font-style-bf">completely</span> (i.e. he cannot split any cup into several days).</p><p>Surely, courseworks are not being written in a single day (in a perfect world of Berland, at least).</p><p>Let's consider some day of Polycarp's work. Consider Polycarp drinks $k$ cups of coffee during this day and caffeine dosages of cups Polycarp drink during this day are $a_{i_1}, a_{i_2}, \dots, a_{i_k}$. Then the first cup he drinks gives him energy to write $a_{i_1}$ pages of coursework, the second cup gives him energy to write $max(0, a_{i_2} - 1)$ pages, the third cup gives him energy to write $max(0, a_{i_3} - 2)$ pages, ..., the $k$-th cup gives him energy to write $max(0, a_{i_k} - k + 1)$ pages.</p><p>If Polycarp doesn't drink coffee during some day, he cannot write coursework at all that day.</p><p>Polycarp has to finish his coursework as soon as possible (spend the minimum number of days to do it). Your task is to find out this number of days or say that it is impossible.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $1 \le m \le 10^9$) — the number of cups of coffee and the number of pages in the coursework.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the caffeine dosage of coffee in the $i$-th cup.</p></div><div class="output-specification"><p>If it is impossible to write the coursework, print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum number of days Polycarp needs to do it.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $1 \le m \le 10^9$) — the number of cups of coffee and the number of pages in the coursework.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the caffeine dosage of coffee in the $i$-th cup.</p>

## Output

<p>If it is impossible to write the coursework, print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum number of days Polycarp needs to do it.</p>





```input1
5 8
2 3 1 1 2
```




```input2
7 10
1 3 4 2 1 4 2
```




```input3
5 15
5 5 5 5 5
```




```input4
5 16
5 5 5 5 5
```




```input5
5 26
5 5 5 5 5
```




```output1
4
```




```output2
2
```




```output3
1
```




```output4
2
```




```output5
-1
```



## Note

<p>In the first example Polycarp can drink fourth cup during first day (and write $1$ page), first and second cups during second day (and write $2 + (3 - 1) = 4$ pages), fifth cup during the third day (and write $2$ pages) and third cup during the fourth day (and write $1$ page) so the answer is $4$. It is obvious that there is no way to write the coursework in three or less days.</p><p>In the second example Polycarp can drink third, fourth and second cups during first day (and write $4 + (2 - 1) + (3 - 2) = 6$ pages) and sixth cup during second day (and write $4$ pages) so the answer is $2$. It is obvious that Polycarp cannot write the whole coursework in one day in this test.</p><p>In the third example Polycarp can drink all cups of coffee during first day and write $5 + (5 - 1) + (5 - 2) + (5 - 3) + (5 - 4) = 15$ pages of coursework.</p><p>In the fourth example Polycarp cannot drink all cups during first day and should drink one of them during the second day. So during first day he will write $5 + (5 - 1) + (5 - 2) + (5 - 3) = 14$ pages of coursework and during second day he will write $5$ pages of coursework. This is enough to complete it.</p><p>In the fifth example Polycarp cannot write the whole coursework at all, even if he will drink one cup of coffee during each day, so the answer is <span class="tex-font-style-tt">-1</span>.</p>
