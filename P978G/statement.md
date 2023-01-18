## Description

<div><p>Petya studies at university. The current academic year finishes with $n$ special days. Petya needs to pass $m$ exams in those special days. The special days in this problem are numbered from $1$ to $n$.</p><p>There are three values about each exam:</p><ul> <li> $s_i$ — the day, when questions for the $i$-th exam will be published, </li><li> $d_i$ — the day of the $i$-th exam ($s_i &lt; d_i$), </li><li> $c_i$ — number of days Petya needs to prepare for the $i$-th exam. For the $i$-th exam Petya should prepare in days between $s_i$ and $d_i-1$, inclusive. </li></ul><p>There are three types of activities for Petya in each day: to spend a day doing nothing (taking a rest), to spend a day passing exactly one exam or to spend a day preparing for exactly one exam. So he can't pass/prepare for multiple exams in a day. He can't mix his activities in a day. If he is preparing for the $i$-th exam in day $j$, then $s_i \le j &lt; d_i$.</p><p>It is allowed to have breaks in a preparation to an exam and to alternate preparations for different exams in consecutive days. So preparation for an exam is not required to be done in consecutive days.</p><p>Find the schedule for Petya to prepare for all exams and pass them, or report that it is impossible.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ $(2 \le n \le 100, 1 \le m \le n)$ — the number of days and the number of exams.</p><p>Each of the following $m$ lines contains three integers $s_i$, $d_i$, $c_i$ $(1 \le s_i &lt; d_i \le n, 1 \le c_i \le n)$ — the day, when questions for the $i$-th exam will be given, the day of the $i$-th exam, number of days Petya needs to prepare for the $i$-th exam. </p><p>Guaranteed, that all the exams will be in different days. Questions for different exams can be given in the same day. It is possible that, in the day of some exam, the questions for other exams are given.</p></div><div class="output-specification"><p>If Petya can not prepare and pass all the exams, print <span class="tex-font-style-tt">-1</span>. In case of positive answer, print $n$ integers, where the $j$-th number is:</p><ul> <li> $(m + 1)$, if the $j$-th day is a day of some exam (recall that in each day no more than one exam is conducted), </li><li> zero, if in the $j$-th day Petya will have a rest, </li><li> $i$ ($1 \le i \le m$), if Petya will prepare for the $i$-th exam in the day $j$ (the total number of days Petya prepares for each exam should be <span class="tex-font-style-bf">strictly</span> equal to the number of days needed to prepare for it).<p>Assume that the exams are numbered in order of appearing in the input, starting from $1$.</p><p>If there are multiple schedules, print any of them.</p></li></ul></div>

## Input

<p>The first line contains two integers $n$ and $m$ $(2 \le n \le 100, 1 \le m \le n)$ — the number of days and the number of exams.</p><p>Each of the following $m$ lines contains three integers $s_i$, $d_i$, $c_i$ $(1 \le s_i &lt; d_i \le n, 1 \le c_i \le n)$ — the day, when questions for the $i$-th exam will be given, the day of the $i$-th exam, number of days Petya needs to prepare for the $i$-th exam. </p><p>Guaranteed, that all the exams will be in different days. Questions for different exams can be given in the same day. It is possible that, in the day of some exam, the questions for other exams are given.</p>

## Output

<p>If Petya can not prepare and pass all the exams, print <span class="tex-font-style-tt">-1</span>. In case of positive answer, print $n$ integers, where the $j$-th number is:</p><ul> <li> $(m + 1)$, if the $j$-th day is a day of some exam (recall that in each day no more than one exam is conducted), </li><li> zero, if in the $j$-th day Petya will have a rest, </li><li> $i$ ($1 \le i \le m$), if Petya will prepare for the $i$-th exam in the day $j$ (the total number of days Petya prepares for each exam should be <span class="tex-font-style-bf">strictly</span> equal to the number of days needed to prepare for it).<p>Assume that the exams are numbered in order of appearing in the input, starting from $1$.</p><p>If there are multiple schedules, print any of them.</p></li></ul>





```input1
5 2
1 3 1
1 5 1

```




```input2
3 2
1 3 1
1 2 1

```




```input3
10 3
4 7 2
1 10 3
8 9 1

```




```output1
1 2 3 0 3 

```




```output2
-1

```




```output3
2 2 2 1 1 0 4 3 4 4 

```



## Note

<p>In the first example Petya can, for example, prepare for exam $1$ in the first day, prepare for exam $2$ in the second day, pass exam $1$ in the third day, relax in the fourth day, and pass exam $2$ in the fifth day. So, he can prepare and pass all exams.</p><p>In the second example, there are three days and two exams. So, Petya can prepare in only one day (because in two other days he should pass exams). Then Petya can not prepare and pass all exams.</p>
