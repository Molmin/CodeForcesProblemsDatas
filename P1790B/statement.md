## Description

<div><p>Taisia has $n$ six-sided dice. Each face of the die is marked with a number from $1$ to $6$, each number from $1$ to $6$ is used once.</p><p>Taisia rolls all $n$ dice at the same time and gets a sequence of values $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 6$), where $a_i$ is the value on the upper face of the $i$-th dice. The sum of this sequence is equal to $s$.</p><p>Suddenly, Taisia's pet cat steals exactly <span class="tex-font-style-bf">one</span> dice with <span class="tex-font-style-bf">maximum</span> value $a_i$ and calculates the sum of the values on the remaining $n-1$ dice, which is equal to $r$.</p><p>You only know the number of dice $n$ and the values of $s$, $r$. Restore a possible sequence $a$ that fulfills the constraints.</p></div><div class="input-specification"><p>The first line contains the integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each testcase is given on a separate line and contains three integers $n$, $s$, $r$ ($2 \le n \le 50$, $1 \le r &lt; s \le 300$).</p><p>It is guaranteed that a solution exists.</p></div><div class="output-specification"><p>For each testcase, print: $n$ integers $a_1, a_2, \ldots, a_n$ in any order. It is guaranteed that such sequence exists.</p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>The first line contains the integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Each testcase is given on a separate line and contains three integers $n$, $s$, $r$ ($2 \le n \le 50$, $1 \le r &lt; s \le 300$).</p><p>It is guaranteed that a solution exists.</p>

## Output

<p>For each testcase, print: $n$ integers $a_1, a_2, \ldots, a_n$ in any order. It is guaranteed that such sequence exists.</p><p>If there are multiple solutions, print any.</p>





```input1|2,4,6,8
7
2 2 1
2 4 2
4 9 5
5 17 11
3 15 10
4 4 3
5 20 15
```




```output1
1 1
2 2 
1 2 2 4
6 4 2 3 2
5 5 5
1 1 1 1
1 4 5 5 5
```


