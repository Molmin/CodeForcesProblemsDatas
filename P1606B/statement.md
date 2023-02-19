## Description

<div><p>Berland State University has received a new update for the operating system. Initially it is installed only on the $1$-st computer.</p><p>Update files should be copied to all $n$ computers. The computers are not connected to the internet, so the only way to transfer update files from one computer to another is to copy them using a patch cable (a cable connecting two computers directly). Only one patch cable can be connected to a computer at a time. Thus, from any computer where the update files are installed, they can be copied to some other computer in exactly one hour.</p><p>Your task is to find the minimum number of hours required to copy the update files to all $n$ computers if there are only $k$ patch cables in Berland State University.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>Each test case consists of a single line that contains two integers $n$ and $k$ ($1 \le k \le n \le 10^{18}$) — the number of computers and the number of patch cables.</p></div><div class="output-specification"><p>For each test case print one integer&nbsp;— the minimum number of hours required to copy the update files to all $n$ computers.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases.</p><p>Each test case consists of a single line that contains two integers $n$ and $k$ ($1 \le k \le n \le 10^{18}$) — the number of computers and the number of patch cables.</p>

## Output

<p>For each test case print one integer&nbsp;— the minimum number of hours required to copy the update files to all $n$ computers.</p>





```input1
4
8 3
6 6
7 1
1 1
```




```output1
4
3
6
0
```



## Note

<p>Let's consider the test cases of the example:</p><ul> <li> $n=8$, $k=3$: <ol> <li> during the first hour, we copy the update files from the computer $1$ to the computer $2$; </li><li> during the second hour, we copy the update files from the computer $1$ to the computer $3$, and from the computer $2$ to the computer $4$; </li><li> during the third hour, we copy the update files from the computer $1$ to the computer $5$, from the computer $2$ to the computer $6$, and from the computer $3$ to the computer $7$; </li><li> during the fourth hour, we copy the update files from the computer $2$ to the computer $8$. </li></ol> </li><li> $n=6$, $k=6$: <ol> <li> during the first hour, we copy the update files from the computer $1$ to the computer $2$; </li><li> during the second hour, we copy the update files from the computer $1$ to the computer $3$, and from the computer $2$ to the computer $4$; </li><li> during the third hour, we copy the update files from the computer $1$ to the computer $5$, and from the computer $2$ to the computer $6$. </li></ol> </li><li> $n=7$, $k=1$: <ol> <li> during the first hour, we copy the update files from the computer $1$ to the computer $2$; </li><li> during the second hour, we copy the update files from the computer $1$ to the computer $3$; </li><li> during the third hour, we copy the update files from the computer $1$ to the computer $4$; </li><li> during the fourth hour, we copy the update files from the computer $4$ to the computer $5$; </li><li> during the fifth hour, we copy the update files from the computer $4$ to the computer $6$; </li><li> during the sixth hour, we copy the update files from the computer $3$ to the computer $7$. </li></ol> </li></ul>
