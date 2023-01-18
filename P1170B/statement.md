## Description

<div><p>Every day Kotlin heroes analyze the statistics of their website. For $n$ days, they wrote out $n$ numbers $a_1, a_2, \dots, a_n$, where $a_i$ is the number of visits on the $i$-th day.</p><p>They believe that a day is bad if there are at least $2$ days before it with a strictly greater number of visits. For example, if $n=8$ and $a=[3, 1, 4, 1, 5, 9, 2, 6]$, then the day $4$ is bad (because $a_4=1$, but there are $a_1=3$ and $a_3=4$). Also, the day with the number $7$ is bad too.</p><p>Write a program that finds the number of bad days.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 2\cdot10^5$), where $n$ is the number of days. The second line contains $n$ positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of website visits on the $i$-th day.</p></div><div class="output-specification"><p>Print the number of bad days, i.e. such days that there are at least two days before it with a strictly greater number of visits.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 2\cdot10^5$), where $n$ is the number of days. The second line contains $n$ positive integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the number of website visits on the $i$-th day.</p>

## Output

<p>Print the number of bad days, i.e. such days that there are at least two days before it with a strictly greater number of visits.</p>





```input1
8
3 1 4 1 5 9 2 6
```




```input2
5
1 1 1 1 1
```




```input3
13
2 7 1 8 2 8 1 8 2 8 4 5 9
```




```output1
2
```




```output2
0
```




```output3
6
```


