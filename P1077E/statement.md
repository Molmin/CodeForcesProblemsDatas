## Description

<div><p>Polycarp has prepared $n$ competitive programming problems. The topic of the $i$-th problem is $a_i$, and some problems' topics may coincide.</p><p>Polycarp has to host several thematic contests. All problems in each contest should have the same topic, and <span class="tex-font-style-bf">all contests should have pairwise distinct topics</span>. He may not use all the problems. It is possible that there are no contests for some topics.</p><p>Polycarp wants to host competitions on consecutive days, one contest per day. Polycarp wants to host a set of contests in such a way that:</p><ul> <li> number of problems in each contest is <span class="tex-font-style-bf">exactly twice</span> as much as in the previous contest (one day ago), the first contest can contain arbitrary number of problems; </li><li> the total number of problems in all the contests should be maximized. </li></ul><p>Your task is to calculate the maximum number of problems in the set of thematic contests. Note, that you should not maximize the number of contests.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of problems Polycarp has prepared.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) where $a_i$ is the topic of the $i$-th problem.</p></div><div class="output-specification"><p>Print one integer — the maximum number of problems in the set of thematic contests.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of problems Polycarp has prepared.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) where $a_i$ is the topic of the $i$-th problem.</p>

## Output

<p>Print one integer — the maximum number of problems in the set of thematic contests.</p>





```input1
18
2 1 2 10 2 10 10 2 2 1 10 10 10 10 1 1 10 10
```




```input2
10
6 6 6 3 6 1000000000 3 3 6 6
```




```input3
3
1337 1337 1337
```




```output1
14
```




```output2
9
```




```output3
3
```



## Note

<p>In the first example the optimal sequence of contests is: $2$ problems of the topic $1$, $4$ problems of the topic $2$, $8$ problems of the topic $10$.</p><p>In the second example the optimal sequence of contests is: $3$ problems of the topic $3$, $6$ problems of the topic $6$.</p><p>In the third example you can take all the problems with the topic $1337$ (the number of such problems is $3$ so the answer is $3$) and host a single contest.</p>
