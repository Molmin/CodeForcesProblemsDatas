## Description

<div><p>A permutation of length $n$ is an array $p=[p_1,p_2,\dots, p_n]$ which contains every integer from $1$ to $n$ (inclusive) exactly once. For example, $p=[4, 2, 6, 5, 3, 1]$ is a permutation of length $6$.</p><p>You are given three integers $n$, $a$ and $b$, where $n$ is an even number. Print any permutation of length $n$ that the minimum among <span class="tex-font-style-bf">all its elements of the left half</span> equals $a$ and the maximum among <span class="tex-font-style-bf">all its elements of the right half</span> equals $b$. Print <span class="tex-font-style-tt">-1</span> if no such permutation exists.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$), the number of test cases in the test. The following $t$ lines contain test case descriptions.</p><p>Each test case description contains three integers $n$, $a$, $b$ ($2 \le n \le 100$; $1 \le a,b \le n$; $a \ne b$), where $n$ is an even number (i.e. $n \bmod 2 = 0$).</p></div><div class="output-specification"><p>For each test case, print a single line containing any suitable permutation. Print <span class="tex-font-style-tt">-1</span> no such permutation exists. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 1000$), the number of test cases in the test. The following $t$ lines contain test case descriptions.</p><p>Each test case description contains three integers $n$, $a$, $b$ ($2 \le n \le 100$; $1 \le a,b \le n$; $a \ne b$), where $n$ is an even number (i.e. $n \bmod 2 = 0$).</p>

## Output

<p>For each test case, print a single line containing any suitable permutation. Print <span class="tex-font-style-tt">-1</span> no such permutation exists. If there are multiple answers, print any of them.</p>





```input1
7
6 2 5
6 1 3
6 4 3
4 2 4
10 5 3
2 1 2
2 2 1
```




```output1
4 2 6 5 3 1
-1
6 4 5 1 3 2 
3 2 4 1 
-1
1 2 
2 1
```


