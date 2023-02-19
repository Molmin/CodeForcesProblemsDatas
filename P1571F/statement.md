## Description

<div><p>Kotlinforces is a web platfrom that hosts programming competitions.</p><p>The staff of Kotlinforces is asked to schedule $n$ programming competitions on the next $m$ days. Each competition is held in multiple stages; the regulations of the $i$-th competition state that this competition should consist of exactly $k_i$ stages, and each stage, starting from the second one, should be scheduled <span class="tex-font-style-bf">exactly $t_i$ days</span> after the previous stage. In other words, if the first stage of the $i$-th competition is scheduled on day $x$, the second stage should be scheduled on day $x+t_i$, the third stage — on day $x+2t_i$, ..., the $k_i$-th stage (which is the last one) — on day $x+(k_i-1)t_i$.</p><p>All $n$ competitions should be scheduled in such a way that they start and finish during the next $m$ days, and on any of these $m$ days, at most one stage of one competition is held (two stages of different competitions should not be scheduled on the same day).</p><p>Is it possible to schedule all $n$ competitions to meet these constraints?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 5000$) — the number of competitions and the number of days, respectively.</p><p>Then $n$ lines follow, each describing a competition which should be scheduled. The $i$-th line contains two integers $k_i$ and $t_i$ ($2 \le k_i \le 5000$; $1 \le t_i \le 2$) — the parameters of the $i$-th competition.</p></div><div class="output-specification"><p>If it is impossible to schedule all $n$ competitions on the next $m$ days so that there is at most one stage during each day, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print $n$ integers. The $i$-th integer should represent the day when the first stage of the $i$-th competition is scheduled; days are numbered from $1$ to $m$. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 5000$) — the number of competitions and the number of days, respectively.</p><p>Then $n$ lines follow, each describing a competition which should be scheduled. The $i$-th line contains two integers $k_i$ and $t_i$ ($2 \le k_i \le 5000$; $1 \le t_i \le 2$) — the parameters of the $i$-th competition.</p>

## Output

<p>If it is impossible to schedule all $n$ competitions on the next $m$ days so that there is at most one stage during each day, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, print $n$ integers. The $i$-th integer should represent the day when the first stage of the $i$-th competition is scheduled; days are numbered from $1$ to $m$. If there are multiple answers, print any of them.</p>





```input1
3 7
3 2
2 2
2 2
```




```input2
1 7
4 2
```




```input3
1 7
5 2
```




```input4
2 4
2 1
2 2
```




```input5
2 5
2 1
2 2
```




```output1
2 5 1
```




```output2
1
```




```output3
-1
```




```output4
-1
```




```output5
4 1
```


