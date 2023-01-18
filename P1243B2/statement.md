## Description

<div><p><span class="tex-font-style-it">This problem is different from the easy version. In this version Ujan makes at most $2n$ swaps. In addition, $k \le 1000, n \le 50$ and it is necessary to print swaps themselves. You can hack this problem if you solve it. But you can hack the previous problem only if you solve both problems.</span></p><p>After struggling and failing many times, Ujan decided to try to clean up his house again. He decided to get his strings in order first.</p><p>Ujan has two <span class="tex-font-style-bf">distinct</span> strings $s$ and $t$ of length $n$ consisting of only of lowercase English characters. He wants to make them equal. Since Ujan is lazy, he will perform the following operation at most $2n$ times: he takes two positions $i$ and $j$ ($1 \le i,j \le n$, the values $i$ and $j$ can be equal or different), and swaps the characters $s_i$ and $t_j$.</p><p>Ujan's goal is to make the strings $s$ and $t$ equal. He does not need to minimize the number of performed operations: <span class="tex-font-style-bf">any</span> sequence of operations of length $2n$ or shorter is suitable.</p></div><div class="input-specification"><p>The first line contains a single integer $k$ ($1 \leq k \leq 1000$), the number of test cases.</p><p>For each of the test cases, the first line contains a single integer $n$ ($2 \leq n \leq 50$), the length of the strings $s$ and $t$. </p><p>Each of the next two lines contains the strings $s$ and $t$, each having length exactly $n$. The strings consist only of lowercase English letters. It is guaranteed that strings are different.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if Ujan can make the two strings equal with at most $2n$ operations and "<span class="tex-font-style-tt">No</span>" otherwise. You can print each letter in any case (upper or lower).</p><p>In the case of "<span class="tex-font-style-tt">Yes</span>" print $m$ ($1 \le m \le 2n$) on the next line, where $m$ is the number of swap operations to make the strings equal. Then print $m$ lines, each line should contain two integers $i, j$ ($1 \le i, j \le n$) meaning that Ujan swaps $s_i$ and $t_j$ during the corresponding operation. You do not need to minimize the number of operations. Any sequence of length not more than $2n$ is suitable.</p></div>

## Input

<p>The first line contains a single integer $k$ ($1 \leq k \leq 1000$), the number of test cases.</p><p>For each of the test cases, the first line contains a single integer $n$ ($2 \leq n \leq 50$), the length of the strings $s$ and $t$. </p><p>Each of the next two lines contains the strings $s$ and $t$, each having length exactly $n$. The strings consist only of lowercase English letters. It is guaranteed that strings are different.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Yes</span>" if Ujan can make the two strings equal with at most $2n$ operations and "<span class="tex-font-style-tt">No</span>" otherwise. You can print each letter in any case (upper or lower).</p><p>In the case of "<span class="tex-font-style-tt">Yes</span>" print $m$ ($1 \le m \le 2n$) on the next line, where $m$ is the number of swap operations to make the strings equal. Then print $m$ lines, each line should contain two integers $i, j$ ($1 \le i, j \le n$) meaning that Ujan swaps $s_i$ and $t_j$ during the corresponding operation. You do not need to minimize the number of operations. Any sequence of length not more than $2n$ is suitable.</p>





```input1
4
5
souse
houhe
3
cat
dog
2
aa
az
3
abc
bca
```




```output1
Yes
1
1 4
No
No
Yes
3
1 2
3 1
2 3
```


