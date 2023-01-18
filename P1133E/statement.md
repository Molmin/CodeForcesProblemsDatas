## Description

<div><p>You are a coach at your local university. There are $n$ students under your supervision, the programming skill of the $i$-th student is $a_i$.</p><p>You have to form $k$ teams for yet another new programming competition. As you know, the more students are involved in competition the more probable the victory of your university is! So you have to form no more than $k$ (and at least one) <span class="tex-font-style-bf">non-empty</span> teams so that the <span class="tex-font-style-bf">total</span> number of students in them is maximized. But you also know that <span class="tex-font-style-bf">each</span> team should be <span class="tex-font-style-it">balanced</span>. It means that the programming skill of each pair of students in <span class="tex-font-style-bf">each</span> team should differ by no more than $5$. Teams are independent from one another (it means that the difference between programming skills of two students from two different teams does not matter).</p><p>It is possible that some students not be included in any team at all.</p><p>Your task is to report the maximum possible <span class="tex-font-style-bf">total</span> number of students in no more than $k$ (and at least one) <span class="tex-font-style-bf">non-empty</span> <span class="tex-font-style-it">balanced</span> teams.</p><p><span class="tex-font-style-bf">If you are Python programmer, consider using PyPy instead of Python when you submit your code.</span></p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$) — the number of students and the maximum number of teams, correspondingly.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is a programming skill of the $i$-th student.</p></div><div class="output-specification"><p>Print one integer — the maximum possible <span class="tex-font-style-bf">total</span> number of students in no more than $k$ (and at least one) <span class="tex-font-style-bf">non-empty</span> <span class="tex-font-style-it">balanced</span> teams.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 5000$) — the number of students and the maximum number of teams, correspondingly.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is a programming skill of the $i$-th student.</p>

## Output

<p>Print one integer — the maximum possible <span class="tex-font-style-bf">total</span> number of students in no more than $k$ (and at least one) <span class="tex-font-style-bf">non-empty</span> <span class="tex-font-style-it">balanced</span> teams.</p>





```input1
5 2
1 2 15 15 15
```




```input2
6 1
36 4 1 25 9 16
```




```input3
4 4
1 10 100 1000
```




```output1
5
```




```output2
2
```




```output3
4
```


