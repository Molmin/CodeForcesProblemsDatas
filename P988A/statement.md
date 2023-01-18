## Description

<div><p>There are $n$ students in a school class, the rating of the $i$-th student on Codehorses is $a_i$. You have to form a team consisting of $k$ students ($1 \le k \le n$) such that the ratings of all team members <span class="tex-font-style-bf">are distinct</span>.</p><p>If it is impossible to form a suitable team, print "<span class="tex-font-style-tt">NO</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">YES</span>", and then print $k$ distinct numbers which should be the indices of students in the team you form. If there are multiple answers, print any of them.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 100$) — the number of students and the size of the team you have to form.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the rating of $i$-th student.</p></div><div class="output-specification"><p>If it is impossible to form a suitable team, print "<span class="tex-font-style-tt">NO</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">YES</span>", and then print $k$ distinct integers from $1$ to $n$ which should be the indices of students in the team you form. All the ratings of the students in the team should be distinct. You may print the indices in any order. If there are multiple answers, print any of them.</p><p>Assume that the students are numbered from $1$ to $n$.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 100$) — the number of students and the size of the team you have to form.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 100$), where $a_i$ is the rating of $i$-th student.</p>

## Output

<p>If it is impossible to form a suitable team, print "<span class="tex-font-style-tt">NO</span>" (without quotes). Otherwise print "<span class="tex-font-style-tt">YES</span>", and then print $k$ distinct integers from $1$ to $n$ which should be the indices of students in the team you form. All the ratings of the students in the team should be distinct. You may print the indices in any order. If there are multiple answers, print any of them.</p><p>Assume that the students are numbered from $1$ to $n$.</p>





```input1
5 3
15 13 15 15 12

```




```input2
5 4
15 13 15 15 12

```




```input3
4 4
20 10 40 30

```




```output1
YES
1 2 5 

```




```output2
NO

```




```output3
YES
1 2 3 4 

```



## Note

<p>All possible answers for the first example: </p><ul> <li> {1 2 5} </li><li> {2 3 5} </li><li> {2 4 5} </li></ul><p>Note that the order does not matter.</p>
