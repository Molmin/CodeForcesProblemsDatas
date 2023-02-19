## Description

<div><p>There are $n$ bags, each bag contains $m$ balls with numbers from $1$ to $m$. For every $i \in [1, m]$, there is exactly one ball with number $i$ in each bag.</p><p>You have to take exactly one ball from each bag (all bags are different, so, for example, taking the ball $1$ from the first bag and the ball $2$ from the second bag is not the same as taking the ball $2$ from the first bag and the ball $1$ from the second bag). After that, you calculate the number of balls with <span class="tex-font-style-bf">odd</span> numbers among the ones you have taken. Let the number of these balls be $F$.</p><p>Your task is to calculate the sum of $F^k$ over all possible ways to take $n$ balls, one from each bag.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing three integers $n$, $m$ and $k$ ($1 \le n, m \le 998244352$; $1 \le k \le 2000$).</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the sum of $F^k$ over all possible ways to take $n$ balls, one from each bag. Since it can be huge, print it modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing three integers $n$, $m$ and $k$ ($1 \le n, m \le 998244352$; $1 \le k \le 2000$).</p>

## Output

<p>For each test case, print one integer&nbsp;— the sum of $F^k$ over all possible ways to take $n$ balls, one from each bag. Since it can be huge, print it modulo $998244353$.</p>





```input1|2,4,6
5
2 3 8
1 1 1
1 5 10
3 7 2000
1337666 42424242 2000
```




```output1
1028
1
3
729229716
652219904
```


