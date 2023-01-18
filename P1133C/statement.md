## Description

<div><p>You are a coach at your local university. There are $n$ students under your supervision, the programming skill of the $i$-th student is $a_i$.</p><p>You have to create a team for a new programming competition. As you know, the more students some team has the more probable its victory is! So you have to create a team with the maximum number of students. But you also know that a team should be <span class="tex-font-style-it">balanced</span>. It means that the programming skill of each pair of students in a created team should differ by no more than $5$.</p><p>Your task is to report the maximum possible number of students in a <span class="tex-font-style-it">balanced</span> team.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of students.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is a programming skill of the $i$-th student.</p></div><div class="output-specification"><p>Print one integer — the maximum possible number of students in a <span class="tex-font-style-it">balanced</span> team.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of students.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is a programming skill of the $i$-th student.</p>

## Output

<p>Print one integer — the maximum possible number of students in a <span class="tex-font-style-it">balanced</span> team.</p>





```input1
6
1 10 17 12 15 2
```




```input2
10
1337 1337 1337 1337 1337 1337 1337 1337 1337 1337
```




```input3
6
1 1000 10000 10 100 1000000000
```




```output1
3
```




```output2
10
```




```output3
1
```



## Note

<p>In the first example you can create a team with skills $[12, 17, 15]$.</p><p>In the second example you can take all students in a team because their programming skills are equal.</p><p>In the third example you can create a team consisting of a single student (and you cannot create a team consisting of at least two students).</p>
