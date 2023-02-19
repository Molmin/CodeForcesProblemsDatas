## Description

<div><p>Naman has two binary strings $s$ and $t$ of length $n$ (a binary string is a string which only consists of the characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>"). He wants to convert $s$ into $t$ using the following operation as few times as possible.</p><p>In one operation, he can choose any subsequence of $s$ and rotate it clockwise once.</p><p>For example, if $s = 1\textbf{1}101\textbf{00}$, he can choose a subsequence corresponding to indices ($1$-based) $\{2, 6, 7 \}$ and rotate them clockwise. The resulting string would then be $s = 1\textbf{0}101\textbf{10}$.</p><p>A string $a$ is said to be a subsequence of string $b$ if $a$ can be obtained from $b$ by deleting some characters without changing the ordering of the remaining characters.</p><p>To perform a clockwise rotation on a sequence $c$ of size $k$ is to perform an operation which sets $c_1:=c_k, c_2:=c_1, c_3:=c_2, \ldots, c_k:=c_{k-1}$ simultaneously.</p><p>Determine the minimum number of operations Naman has to perform to convert $s$ into $t$ or say that it is impossible. </p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(1 \le n \le 10^6)$&nbsp;— the length of the strings.</p><p>The second line contains the binary string $s$ of length $n$.</p><p>The third line contains the binary string $t$ of length $n$.</p></div><div class="output-specification"><p>If it is impossible to convert $s$ to $t$ after any number of operations, print $-1$.</p><p>Otherwise, print the minimum number of operations required.</p></div>

## Input

<p>The first line contains a single integer $n$ $(1 \le n \le 10^6)$&nbsp;— the length of the strings.</p><p>The second line contains the binary string $s$ of length $n$.</p><p>The third line contains the binary string $t$ of length $n$.</p>

## Output

<p>If it is impossible to convert $s$ to $t$ after any number of operations, print $-1$.</p><p>Otherwise, print the minimum number of operations required.</p>





```input1
6
010000
000001
```




```input2
10
1111100000
0000011111
```




```input3
8
10101010
01010101
```




```input4
10
1111100000
1111100001
```




```output1
1
```




```output2
5
```




```output3
1
```




```output4
-1
```



## Note

<p>In the first test, Naman can choose the subsequence corresponding to indices $\{2, 6\}$ and rotate it once to convert $s$ into $t$.</p><p>In the second test, he can rotate the subsequence corresponding to all indices $5$ times. It can be proved, that it is the minimum required number of operations.</p><p>In the last test, it is impossible to convert $s$ into $t$.</p>
