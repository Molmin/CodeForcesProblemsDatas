## Description

<div><p>Some number of people (this number is even) have stood in a circle. The people stand in the circle evenly. They are numbered clockwise starting from a person with the number $1$. Each person is looking through the circle's center at the opposite person.</p><center> <img class="tex-graphics" src="file://sAjSaZRY.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">A sample of a circle of $6$ persons. The orange arrows indicate who is looking at whom.</span> </center><p>You don't know the exact number of people standing in the circle (but this number is even, no doubt). It is known that the person with the number $a$ is looking at the person with the number $b$ (and vice versa, of course). What is the number associated with a person being looked at by the person with the number $c$? If, for the specified $a$, $b$, and $c$, no such circle exists, output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing three <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$ ($1 \le a,b,c \le 10^8$).</p></div><div class="output-specification"><p>For each test case output in a separate line a single integer $d$ — the number of the person being looked at by the person with the number $c$ in a circle such that the person with the number $a$ is looking at the person with the number $b$. If there are multiple solutions, print any of them. Output $-1$ if there's no circle meeting the given conditions.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one line containing three <span class="tex-font-style-bf">distinct</span> integers $a$, $b$, $c$ ($1 \le a,b,c \le 10^8$).</p>

## Output

<p>For each test case output in a separate line a single integer $d$ — the number of the person being looked at by the person with the number $c$ in a circle such that the person with the number $a$ is looking at the person with the number $b$. If there are multiple solutions, print any of them. Output $-1$ if there's no circle meeting the given conditions.</p>





```input1
7
6 2 4
2 3 1
2 4 10
5 3 4
1 3 2
2 5 4
4 3 2
```




```output1
8
-1
-1
-1
4
1
-1
```



## Note

<p>In the first test case, there's a desired circle of $8$ people. The person with the number $6$ will look at the person with the number $2$ and the person with the number $8$ will look at the person with the number $4$.</p><p>In the second test case, there's no circle meeting the conditions. If the person with the number $2$ is looking at the person with the number $3$, the circle consists of $2$ people because these persons are neighbors. But, in this case, they must have the numbers $1$ and $2$, but it doesn't meet the problem's conditions.</p><p>In the third test case, the only circle with the persons with the numbers $2$ and $4$ looking at each other consists of $4$ people. Therefore, the person with the number $10$ doesn't occur in the circle.</p>
