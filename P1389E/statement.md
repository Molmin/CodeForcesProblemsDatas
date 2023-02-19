## Description

<div><p>Berland year consists of $m$ months with $d$ days each. Months are numbered from $1$ to $m$. Berland week consists of $w$ days. The first day of the year is also the first day of the week. Note that the last week of the year might be shorter than $w$ days.</p><p>A pair $(x, y)$ such that $x &lt; y$ is ambiguous if day $x$ of month $y$ is the same day of the week as day $y$ of month $x$.</p><p>Count the number of ambiguous pairs.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains three integers $m$, $d$ and $w$ ($1 \le m, d, w \le 10^9$)&nbsp;— the number of months in a year, the number of days in a month and the number of days in a week.</p></div><div class="output-specification"><p>Print $t$ integers&nbsp;— for each testcase output the number of pairs $(x, y)$ such that $x &lt; y$ and day $x$ of month $y$ is the same day of the week as day $y$ of month $x$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each of the next $t$ lines contains three integers $m$, $d$ and $w$ ($1 \le m, d, w \le 10^9$)&nbsp;— the number of months in a year, the number of days in a month and the number of days in a week.</p>

## Output

<p>Print $t$ integers&nbsp;— for each testcase output the number of pairs $(x, y)$ such that $x &lt; y$ and day $x$ of month $y$ is the same day of the week as day $y$ of month $x$.</p>





```input1
5
6 7 4
10 7 12
12 30 7
1 1 1
3247834 10298779 625324
```




```output1
6
9
5
0
116461800
```



## Note

<p>Here are the pairs for the first test case: </p><center> <img class="tex-graphics" src="file://GmZF4Aq6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
