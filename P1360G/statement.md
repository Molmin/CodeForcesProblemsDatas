## Description

<div><p>You are given four positive integers $n$, $m$, $a$, $b$ ($1 \le b \le n \le 50$; $1 \le a \le m \le 50$). Find any such rectangular matrix of size $n \times m$ that satisfies all of the following conditions:</p><ul> <li> each row of the matrix contains exactly $a$ ones; </li><li> each column of the matrix contains exactly $b$ ones; </li><li> all other elements are zeros. </li></ul><p>If the desired matrix does not exist, indicate this.</p><p>For example, for $n=3$, $m=6$, $a=2$, $b=1$, there exists a matrix satisfying the conditions above:</p><p>$$ \begin{vmatrix} 0 &amp; 1 &amp; 0 &amp; 0 &amp; 0 &amp; 1 \\ 1 &amp; 0 &amp; 0 &amp; 1 &amp; 0 &amp; 0 \\ 0 &amp; 0 &amp; 1 &amp; 0 &amp; 1 &amp; 0 \end{vmatrix} $$</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case is described by four positive integers $n$, $m$, $a$, $b$ ($1 \le b \le n \le 50$; $1 \le a \le m \le 50$), where $n$ and $m$ are the sizes of the matrix, and $a$ and $b$ are the number of ones for rows and columns, respectively.</p></div><div class="output-specification"><p>For each test case print:</p><ul> <li> "YES" (without quotes) and the required matrix (if there are several answers, print any) if it exists, or </li><li> "NO" (without quotes) if it does not exist. </li></ul><p>To print the matrix $n \times m$, print $n$ rows, each of which consists of $m$ numbers $0$ or $1$ describing a row of the matrix. Numbers must be printed <span class="tex-font-style-bf">without spaces</span>.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case is described by four positive integers $n$, $m$, $a$, $b$ ($1 \le b \le n \le 50$; $1 \le a \le m \le 50$), where $n$ and $m$ are the sizes of the matrix, and $a$ and $b$ are the number of ones for rows and columns, respectively.</p>

## Output

<p>For each test case print:</p><ul> <li> "YES" (without quotes) and the required matrix (if there are several answers, print any) if it exists, or </li><li> "NO" (without quotes) if it does not exist. </li></ul><p>To print the matrix $n \times m$, print $n$ rows, each of which consists of $m$ numbers $0$ or $1$ describing a row of the matrix. Numbers must be printed <span class="tex-font-style-bf">without spaces</span>.</p>





```input1
5
3 6 2 1
2 2 2 1
2 2 2 2
4 4 2 2
2 1 1 2
```




```output1
YES
010001
100100
001010
NO
YES
11
11
YES
1100
1100
0011
0011
YES
1
1
```


