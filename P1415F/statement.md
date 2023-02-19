## Description

<div><p>You live on a number line. You are initially (at time moment $t = 0$) located at point $x = 0$. There are $n$ events of the following type: at time $t_i$ a small cake appears at coordinate $x_i$. To collect this cake, you have to be at this coordinate at this point, otherwise the cake spoils immediately. No two cakes appear at the same time and no two cakes appear at the same coordinate.</p><p>You can move with the speed of $1$ length unit per one time unit. Also, at any moment you can create a clone of yourself at the same point where you are located. The clone can't move, but it will collect the cakes appearing at this position for you. The clone <span class="tex-font-style-bf">disappears</span> when you create another clone. If the new clone is created at time moment $t$, the old clone can collect the cakes that appear before or at the time moment $t$, and the new clone can collect the cakes that appear at or after time moment $t$.</p><p>Can you collect all the cakes (by yourself or with the help of clones)?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the number of cakes.</p><p>Each of the next $n$ lines contains two integers $t_i$ and $x_i$ ($1 \le t_i \le 10^9$, $-10^9 \le x_i \le 10^9$)&nbsp;— the time and coordinate of a cake's appearance.</p><p>All times are distinct and are given in increasing order, all the coordinates are <span class="tex-font-style-bf">distinct</span>.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if you can collect all cakes, otherwise print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 5000$)&nbsp;— the number of cakes.</p><p>Each of the next $n$ lines contains two integers $t_i$ and $x_i$ ($1 \le t_i \le 10^9$, $-10^9 \le x_i \le 10^9$)&nbsp;— the time and coordinate of a cake's appearance.</p><p>All times are distinct and are given in increasing order, all the coordinates are <span class="tex-font-style-bf">distinct</span>.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if you can collect all cakes, otherwise print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3
2 2
5 5
6 1
```




```input2
3
1 0
5 5
6 2
```




```input3
3
2 1
5 5
6 0
```




```output1
YES
```




```output2
YES
```




```output3
NO
```



## Note

<p>In the first example you should start moving towards $5$ right away, leaving a clone at position $1$ at time moment $1$, and collecting the cake at position $2$ at time moment $2$. At time moment $5$ you are at the position $5$ and collect a cake there, your clone collects the last cake at time moment $6$.</p><p>In the second example you have to leave a clone at position $0$ and start moving towards position $5$. At time moment $1$ the clone collects a cake. At time moment $2$ you should create a new clone at the current position $2$, it will collect the last cake in future. You will collect the second cake at position $5$.</p><p>In the third example there is no way to collect all cakes.</p>
