## Description

<div><p>Polycarp plans to undergo a full physical examination at his local clinic. There are $n$ doctors, numbered from $1$ to $n$. The $i$-th doctor takes patients from minute $L_i$ to minute $R_i$, so Polycarp can visit him at any minute in this range. It takes each doctor exactly one minute to examine Polycarp's health.</p><p>Polycarp wants to arrive at the clinic at some minute $x$ and visit all $n$ doctors in some order <span class="tex-font-style-bf">without waiting or visiting any doctor several times</span>.</p><p>More formally, he chooses an integer $x$ and a permutation $p_1, p_2, \dots, p_n$ (a sequence of $n$ integers from $1$ to $n$ such that each integer appears exactly once), then proceeds to visit: </p><ul> <li> doctor $p_1$ at minute $x$; </li><li> doctor $p_2$ at minute $x+1$; </li><li> ... </li><li> doctor $p_n$ at minute $x+n-1$. </li></ul><p>The $p_i$-th doctor should be able to take patients at minute $x+i-1$, so the following should hold: $L[p_i] \le x + i - 1 \le R[p_i]$.</p><p>Determine if it's possible for Polycarp to choose such a minute $x$ and a permutation $p$ that he'll be able to visit all $n$ doctors in without waiting or visiting any doctor several times. If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of doctors.</p><p>The second line of the testcase contains $n$ integers $L_1, L_2, \dots L_n$ ($1 \le L_i \le 10^9$).</p><p>The third line of the testcase contains $n$ integers $R_1, R_2, \dots R_n$ ($L_i \le R_i \le 10^9$).</p><p>The sum of $n$ over all testcases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each testcase print an answer.</p><p>If there exists such a minute $x$ and a permutation $p$ that Polycarp is able to visit all $n$ doctors without waiting or visiting any doctor several times, then print $x$ in the first line and a permutation $p$ in the second line. If there are multiple answers, print any of them.</p><p>Otherwise, print $-1$ in the only line.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of the testcase contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of doctors.</p><p>The second line of the testcase contains $n$ integers $L_1, L_2, \dots L_n$ ($1 \le L_i \le 10^9$).</p><p>The third line of the testcase contains $n$ integers $R_1, R_2, \dots R_n$ ($L_i \le R_i \le 10^9$).</p><p>The sum of $n$ over all testcases doesn't exceed $10^5$.</p>

## Output

<p>For each testcase print an answer.</p><p>If there exists such a minute $x$ and a permutation $p$ that Polycarp is able to visit all $n$ doctors without waiting or visiting any doctor several times, then print $x$ in the first line and a permutation $p$ in the second line. If there are multiple answers, print any of them.</p><p>Otherwise, print $-1$ in the only line.</p>





```input1
5
3
2 3 1
3 3 2
8
6 6 5 4 9 4 3 6
7 6 10 6 9 6 6 8
2
4 2
4 2
3
2 2 2
3 3 3
1
5
10
```




```output1
1
3 1 2 
3
7 4 6 2 1 8 5 3 
-1
-1
7
1
```



## Note

<p>In the third testcase it's impossible to visit all doctors, because Polycarp has to visit doctor $2$ at minute $2$ and doctor $1$ at minute $4$. However, that would require him to wait a minute between the visits, which is not allowed.</p><p>In the fourth testcase all doctors take patients in the span of $2$ minutes. However, since there are three of them, Polycarp can't visit them all.</p>
