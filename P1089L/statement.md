## Description

<div><p>The kingdom of Lazyland is the home to $n$ idlers. These idlers are incredibly lazy and create many problems to their ruler, the mighty King of Lazyland. </p><p>Today $k$ important jobs for the kingdom ($k \le n$) should be performed. Every job should be done by one person and every person can do at most one job. The King allowed every idler to choose one job they wanted to do and the $i$-th idler has chosen the job $a_i$. </p><p>Unfortunately, some jobs may not be chosen by anyone, so the King has to persuade some idlers to choose another job. The King knows that it takes $b_i$ minutes to persuade the $i$-th idler. He asked his minister of labour to calculate the minimum total time he needs to spend persuading the idlers to get all the jobs done. Can you help him? </p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$)&nbsp;— the number of idlers and the number of jobs.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le k$)&nbsp;— the jobs chosen by each idler.</p><p>The third line of the input contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the time the King needs to spend to persuade the $i$-th idler.</p></div><div class="output-specification"><p>The only line of the output should contain one number&nbsp;— the minimum total time the King needs to spend persuading the idlers to get all the jobs done.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le k \le n \le 10^5$)&nbsp;— the number of idlers and the number of jobs.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le k$)&nbsp;— the jobs chosen by each idler.</p><p>The third line of the input contains $n$ integers $b_1, b_2, \ldots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the time the King needs to spend to persuade the $i$-th idler.</p>

## Output

<p>The only line of the output should contain one number&nbsp;— the minimum total time the King needs to spend persuading the idlers to get all the jobs done.</p>





```input1
8 7
1 1 3 1 5 3 7 1
5 7 4 8 1 3 5 2
```




```input2
3 3
3 1 2
5 3 4
```




```output1
10
```




```output2
0
```



## Note

<p>In the first example the optimal plan is to persuade idlers 1, 6, and 8 to do jobs 2, 4, and 6.</p><p>In the second example each job was chosen by some idler, so there is no need to persuade anyone.</p>
