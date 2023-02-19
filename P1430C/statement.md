## Description

<div><p>Numbers $1, 2, 3, \dots n$ (each integer from $1$ to $n$ once) are written on a board. In one operation you can erase any two numbers $a$ and $b$ from the board and write one integer $\frac{a + b}{2}$ <span class="tex-font-style-it">rounded up</span> instead.</p><p>You should perform the given operation $n - 1$ times and make the resulting number that will be left on the board as small as possible. </p><p>For example, if $n = 4$, the following course of action is optimal:</p><ol> <li> choose $a = 4$ and $b = 2$, so the new number is $3$, and the whiteboard contains $[1, 3, 3]$; </li><li> choose $a = 3$ and $b = 3$, so the new number is $3$, and the whiteboard contains $[1, 3]$; </li><li> choose $a = 1$ and $b = 3$, so the new number is $2$, and the whiteboard contains $[2]$. </li></ol><p>It's easy to see that after $n - 1$ operations, there will be left only one number. Your goal is to minimize it.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of integers written on the board initially.</p><p>It's guaranteed that the total sum of $n$ over test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, in the first line, print the minimum possible number left on the board after $n - 1$ operations. Each of the next $n - 1$ lines should contain two integers&nbsp;— numbers $a$ and $b$ chosen and erased in each operation.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The only line of each test case contains one integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;— the number of integers written on the board initially.</p><p>It's guaranteed that the total sum of $n$ over test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, in the first line, print the minimum possible number left on the board after $n - 1$ operations. Each of the next $n - 1$ lines should contain two integers&nbsp;— numbers $a$ and $b$ chosen and erased in each operation.</p>





```input1
1
4
```




```output1
2
2 4
3 3
3 1
```


