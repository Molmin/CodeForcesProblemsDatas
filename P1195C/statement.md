## Description

<div><p>Finally, a basketball court has been opened in SIS, so Demid has decided to hold a basketball exercise session. $2 \cdot n$ students have come to Demid's exercise session, and he lined up them into two rows of the same size (there are exactly $n$ people in each row). Students are numbered from $1$ to $n$ in each row in order from left to right.</p><center> <img class="tex-graphics" src="file://jcOoml43.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Now Demid wants to choose a team to play basketball. He will choose players from left to right, and the index of each chosen player (excluding the first one <span class="tex-font-style-bf">taken</span>) will be strictly greater than the index of the previously chosen player. To avoid giving preference to one of the rows, Demid chooses students in such a way that no consecutive chosen students belong to the same row. The first student can be chosen among all $2n$ students (there are no additional constraints), and a team can consist of any number of students. </p><p>Demid thinks, that in order to compose a perfect team, he should choose students in such a way, that the total height of all chosen students is maximum possible. Help Demid to find the maximum possible total height of players in a team he can choose.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of students in each row.</p><p>The second line of the input contains $n$ integers $h_{1, 1}, h_{1, 2}, \ldots, h_{1, n}$ ($1 \le h_{1, i} \le 10^9$), where $h_{1, i}$ is the height of the $i$-th student in the first row.</p><p>The third line of the input contains $n$ integers $h_{2, 1}, h_{2, 2}, \ldots, h_{2, n}$ ($1 \le h_{2, i} \le 10^9$), where $h_{2, i}$ is the height of the $i$-th student in the second row.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible total height of players in a team Demid can choose.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of students in each row.</p><p>The second line of the input contains $n$ integers $h_{1, 1}, h_{1, 2}, \ldots, h_{1, n}$ ($1 \le h_{1, i} \le 10^9$), where $h_{1, i}$ is the height of the $i$-th student in the first row.</p><p>The third line of the input contains $n$ integers $h_{2, 1}, h_{2, 2}, \ldots, h_{2, n}$ ($1 \le h_{2, i} \le 10^9$), where $h_{2, i}$ is the height of the $i$-th student in the second row.</p>

## Output

<p>Print a single integer — the maximum possible total height of players in a team Demid can choose.</p>





```input1
5
9 3 5 7 3
5 8 1 4 5
```




```input2
3
1 2 9
10 1 1
```




```input3
1
7
4
```




```output1
29
```




```output2
19
```




```output3
7
```



## Note

<p>In the first example Demid can choose the following team as follows: </p><center> <img class="tex-graphics" src="file://rI6ePXiH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second example Demid can choose the following team as follows: </p><center> <img class="tex-graphics" src="file://4yiipzuz.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
