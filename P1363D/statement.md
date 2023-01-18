## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Ayush devised a new scheme to set the password of his lock. The lock has $k$ slots where each slot can hold integers from $1$ to $n$. The password $P$ is a sequence of $k$ integers each in the range $[1, n]$, $i$-th element of which goes into the $i$-th slot of the lock.</p><p>To set the password of his lock, Ayush comes up with an array $A$ of $n$ integers each in the range $[1, n]$ (not necessarily distinct). He then picks $k$ <span class="tex-font-style-bf">non-empty mutually disjoint</span> subsets of indices $S_1, S_2, ..., S_k$ $(S_i \underset{i \neq j} \cap S_j = \emptyset)$ and sets his password as $P_i = \max\limits_{j \notin S_i} A[j]$. In other words, the $i$-th integer in the password is equal to the maximum over all elements of $A$ whose indices do not belong to $S_i$.</p><p>You are given the subsets of indices chosen by Ayush. You need to guess the password. To make a query, you can choose a non-empty subset of indices of the array and ask the maximum of all elements of the array with index in this subset. <span class="tex-font-style-bf">You can ask no more than 12 queries</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10)$&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ $(2 \leq n \leq 1000, 1 \leq k \leq n)$&nbsp;— the size of the array and the number of subsets. $k$ lines follow. The $i$-th line contains an integer $c$ $(1 \leq c \lt n)$&nbsp;— the size of subset $S_i$, followed by $c$ distinct integers in the range $[1, n]$ &nbsp;— indices from the subset $S_i$.</p><p><span class="tex-font-style-bf">It is guaranteed that the intersection of any two subsets is empty.</span></p></div><div><h2>Interaction</h2><p>To ask a query print a single line: </p><ul> <li> In the beginning print "<span class="tex-font-style-tt">? c</span> " (without quotes) where $c$ $(1 \leq c \leq n)$ denotes the size of the subset of indices being queried, followed by $c$ <span class="tex-font-style-bf">distinct</span> space-separated integers in the range $[1, n]$. </li></ul><p>For each query, you will receive an integer $x$&nbsp;— the maximum of value in the array among all the indices queried. If the subset of indices queried is invalid or you exceeded the number of queries (for example one of the indices is greater than $n$) then you will get $x = -1$. In this case, you should terminate the program immediately.</p><p>When you have guessed the password, print a single line "<span class="tex-font-style-tt">!</span> " (without quotes), followed by $k$ space-separated integers &nbsp;— the password sequence.</p><p>Guessing the password does <span class="tex-font-style-bf">not</span> count towards the number of queries asked.</p><p><span class="tex-font-style-bf">After this, you should read a string</span>. If you guess the password correctly, you will receive the string "<span class="tex-font-style-tt">Correct</span>". In this case, you should continue solving the remaining test cases. If the guessed password is incorrect, you will receive the string "<span class="tex-font-style-tt">Incorrect</span>". In this case, you should terminate the program immediately.</p><p><span class="tex-font-style-bf">The interactor is not adaptive.</span> The array $A$ does not change with queries.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack the solution use the following test format:</p><p>The first line of the input should contain a single integer $t$ $(1 \leq t \leq 10)$&nbsp;— the number of test cases. </p><p>The first line of each test case should contain two integers $n$ and $k$ $(2 \leq n \leq 1000, 1 \leq k \leq n)$&nbsp;— the size of the array and the number of subsets. The next line should consist of $n$ space separated integers in the range $[1, n]$&nbsp;— the array $A$. $k$ lines should follow. The $i$-th line should contain an integer $c$ $(1 \leq c \lt n)$&nbsp;— the size of subset $S_i$, followed by $c$ distinct integers in the range $[1, n]$ &nbsp;— indices from the subset $S_i$.</p><p><span class="tex-font-style-bf">The intersection of any two subsets has to be empty.</span></p></div>

## Input

<p>The first line of the input contains a single integer $t$ $(1 \leq t \leq 10)$&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ $(2 \leq n \leq 1000, 1 \leq k \leq n)$&nbsp;— the size of the array and the number of subsets. $k$ lines follow. The $i$-th line contains an integer $c$ $(1 \leq c \lt n)$&nbsp;— the size of subset $S_i$, followed by $c$ distinct integers in the range $[1, n]$ &nbsp;— indices from the subset $S_i$.</p><p><span class="tex-font-style-bf">It is guaranteed that the intersection of any two subsets is empty.</span></p>





```input1
1
4 2
2 1 3
2 2 4

1

2

3

4

Correct
```




```output1
? 1 1

? 1 2

? 1 3

? 1 4

! 4 3
```



## Note

<p>The array $A$ in the example is $[1, 2, 3, 4]$. The length of the password is $2$. The first element of the password is the maximum of $A[2]$, $A[4]$ (since the first subset contains indices $1$ and $3$, we take maximum over remaining indices). The second element of the password is the maximum of $A[1]$, $A[3]$ (since the second subset contains indices $2$, $4$).</p><p><span class="tex-font-style-bf">Do not forget</span> to read the string "<span class="tex-font-style-tt">Correct</span>" / "<span class="tex-font-style-tt">Incorrect</span>" after guessing the password.</p>
