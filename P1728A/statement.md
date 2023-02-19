## Description

<div><p><span class="tex-font-style-it">The title is a reference to the very first Educational Round from our writers team, Educational Round 18.</span></p><p>There is a bag, containing colored balls. There are $n$ different colors of balls, numbered from $1$ to $n$. There are $\mathit{cnt}_i$ balls of color $i$ in the bag. The total amount of balls in the bag is odd (e. g. $\mathit{cnt}_1 + \mathit{cnt}_2 + \dots + \mathit{cnt}_n$ is odd).</p><p>In one move, you can choose two balls <span class="tex-font-style-bf">with different colors</span> and take them out of the bag.</p><p>At some point, all the remaining balls in the bag will have the same color. That's when you can't make moves anymore.</p><p>Find any possible color of the remaining balls.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 20$)&nbsp;— the number of colors.</p><p>The second line contains $n$ integers $\mathit{cnt}_1, \mathit{cnt}_2, \dots, \mathit{cnt}_n$ ($1 \le \mathit{cnt}_i \le 100$)&nbsp;— the amount of balls of each color in the bag.</p><p>The total amount of balls in the bag is odd (e. g. $\mathit{cnt}_1 + \mathit{cnt}_2 + \dots + \mathit{cnt}_n$ is odd).</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— any possible color of the remaining balls, after you made some moves and can't make moves anymore.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 20$)&nbsp;— the number of colors.</p><p>The second line contains $n$ integers $\mathit{cnt}_1, \mathit{cnt}_2, \dots, \mathit{cnt}_n$ ($1 \le \mathit{cnt}_i \le 100$)&nbsp;— the amount of balls of each color in the bag.</p><p>The total amount of balls in the bag is odd (e. g. $\mathit{cnt}_1 + \mathit{cnt}_2 + \dots + \mathit{cnt}_n$ is odd).</p>

## Output

<p>For each testcase, print a single integer&nbsp;— any possible color of the remaining balls, after you made some moves and can't make moves anymore.</p>





```input1|2,3,6,7
3
3
1 1 1
1
9
2
4 7
```




```output1
3
1
2
```



## Note

<p>In the first testcase, your first and only move can be one of the following: </p><ul> <li> take balls with colors $1$ and $2$; </li><li> take balls with colors $1$ and $3$; </li><li> take balls with colors $2$ and $3$. </li></ul><p>After the move, exactly one ball will remain. Its color can be $3, 2$ or $1$ depending on the move.</p><p>In the second testcase, you can't make moves at all&nbsp;— there is only color of balls already. This color is $1$.</p><p>In the third testcase, you can keep removing one ball of color $1$ and one ball of color $2$ until there are no more balls of color $1$. At the end, three balls of color $2$ remain.</p>
