## Description

<div><p>There are $n$ students at your university. The programming skill of the $i$-th student is $a_i$. As a coach, you want to divide them into teams to prepare them for the upcoming ICPC finals. Just imagine how good this university is if it has $2 \cdot 10^5$ students ready for the finals!</p><p>Each team should consist of <span class="tex-font-style-bf">at least three students</span>. Each student should belong to <span class="tex-font-style-bf">exactly one team</span>. The <span class="tex-font-style-it">diversity</span> of a team is the difference between the <span class="tex-font-style-bf">maximum</span> programming skill of some student that belongs to this team and the <span class="tex-font-style-bf">minimum</span> programming skill of some student that belongs to this team (in other words, if the team consists of $k$ students with programming skills $a[i_1], a[i_2], \dots, a[i_k]$, then the <span class="tex-font-style-it">diversity</span> of this team is $\max\limits_{j=1}^{k} a[i_j] - \min\limits_{j=1}^{k} a[i_j]$).</p><p>The total <span class="tex-font-style-it">diversity</span> is the sum of <span class="tex-font-style-it">diversities</span> of all teams formed.</p><p>Your task is to minimize the total <span class="tex-font-style-it">diversity</span> of the division of students and find the optimal way to divide the students.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($3 \le n \le 2 \cdot 10^5$) — the number of students.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the programming skill of the $i$-th student.</p></div><div class="output-specification"><p>In the first line print two integers $res$ and $k$ — the minimum total <span class="tex-font-style-it">diversity</span> of the division of students and the number of teams in your division, correspondingly.</p><p>In the second line print $n$ integers $t_1, t_2, \dots, t_n$ ($1 \le t_i \le k$), where $t_i$ is the number of team to which the $i$-th student belong.</p><p>If there are multiple answers, you can print any. Note that you don't need to minimize the number of teams. Each team should consist of <span class="tex-font-style-bf">at least three students</span>.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($3 \le n \le 2 \cdot 10^5$) — the number of students.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the programming skill of the $i$-th student.</p>

## Output

<p>In the first line print two integers $res$ and $k$ — the minimum total <span class="tex-font-style-it">diversity</span> of the division of students and the number of teams in your division, correspondingly.</p><p>In the second line print $n$ integers $t_1, t_2, \dots, t_n$ ($1 \le t_i \le k$), where $t_i$ is the number of team to which the $i$-th student belong.</p><p>If there are multiple answers, you can print any. Note that you don't need to minimize the number of teams. Each team should consist of <span class="tex-font-style-bf">at least three students</span>.</p>





```input1
5
1 1 3 4 2
```




```input2
6
1 5 12 13 2 15
```




```input3
10
1 2 5 129 185 581 1041 1909 1580 8150
```




```output1
3 1
1 1 1 1 1
```




```output2
7 2
2 2 1 1 2 1
```




```output3
7486 3
3 3 3 2 2 2 2 1 1 1
```



## Note

<p>In the first example, there is only one team with skills $[1, 1, 2, 3, 4]$ so the answer is $3$. It can be shown that you cannot achieve a better answer.</p><p>In the second example, there are two teams with skills $[1, 2, 5]$ and $[12, 13, 15]$ so the answer is $4 + 3 = 7$.</p><p>In the third example, there are three teams with skills $[1, 2, 5]$, $[129, 185, 581, 1041]$ and $[1580, 1909, 8150]$ so the answer is $4 + 912 + 6570 = 7486$.</p>
