## Description

<div><p>Pak Chanek has $n$ blank heart-shaped cards. Card $1$ is attached directly to the wall while each of the other cards is hanging onto exactly one other card by a piece of string. Specifically, card $i$ ($i &gt; 1$) is hanging onto card $p_i$ ($p_i &lt; i$).</p><p>In the very beginning, Pak Chanek must write one integer number on each card. He does this by choosing any permutation $a$ of $[1, 2, \dots, n]$. Then, the number written on card $i$ is $a_i$.</p><p>After that, Pak Chanek must do the following operation $n$ times while maintaining a sequence $s$ (which is initially empty):</p><ol> <li> Choose a card $x$ such that no other cards are hanging onto it. </li><li> Append the number written on card $x$ to the end of $s$. </li><li> If $x \neq 1$ and the number on card $p_x$ is larger than the number on card $x$, replace the number on card $p_x$ with the number on card $x$. </li><li> Remove card $x$. </li></ol><p>After that, Pak Chanek will have a sequence $s$ with $n$ elements. What is the maximum length of the longest non-decreasing subsequence$^\dagger$ of $s$ at the end if Pak Chanek does all the steps optimally?</p><p>$^\dagger$ A sequence $b$ is a subsequence of a sequence $c$ if $b$ can be obtained from $c$ by deletion of several (possibly, zero or all) elements. For example, $[3,1]$ is a subsequence of $[3,2,1]$, $[4,3,1]$ and $[3,1]$, but not $[1,3,3,7]$ and $[3,10,4]$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$) — the number of heart-shaped cards.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \dots, p_n$ ($1 \le p_i &lt; i$) describing which card that each card hangs onto.</p></div><div class="output-specification"><p>Print a single integer — the maximum length of the longest non-decreasing subsequence of $s$ at the end if Pak Chanek does all the steps optimally.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$) — the number of heart-shaped cards.</p><p>The second line contains $n - 1$ integers $p_2, p_3, \dots, p_n$ ($1 \le p_i &lt; i$) describing which card that each card hangs onto.</p>

## Output

<p>Print a single integer — the maximum length of the longest non-decreasing subsequence of $s$ at the end if Pak Chanek does all the steps optimally.</p>





```input1
6
1 2 1 4 2
```




```input2
2
1
```




```output1
4
```




```output2
2
```



## Note

<p>The following is the structure of the cards in the first example.</p><p><img class="tex-graphics" src="file://bOGYnosi.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Pak Chanek can choose the permutation $a = [1, 5, 4, 3, 2, 6]$.</p><p><img class="tex-graphics" src="file://Uz87ou7F.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Let $w_i$ be the number written on card $i$. Initially, $w_i = a_i$. Pak Chanek can do the following operations in order:</p><ol> <li> Select card $5$. Append $w_5 = 2$ to the end of $s$. As $w_4 &gt; w_5$, the value of $w_4$ becomes $2$. Remove card $5$. After this operation, $s = [2]$. </li><li> Select card $6$. Append $w_6 = 6$ to the end of $s$. As $w_2 \leq w_6$, the value of $w_2$ is left unchanged. Remove card $6$. After this operation, $s = [2, 6]$. </li><li> Select card $4$. Append $w_4 = 2$ to the end of $s$. As $w_1 \leq w_4$, the value of $w_1$ is left unchanged. Remove card $4$. After this operation, $s = [2, 6, 2]$. </li><li> Select card $3$. Append $w_3 = 4$ to the end of $s$. As $w_2 &gt; w_3$, the value of $w_2$ becomes $4$. Remove card $3$. After this operation, $s = [2, 6, 2, 4]$. </li><li> Select card $2$. Append $w_2 = 4$ to the end of $s$. As $w_1 \leq w_2$, the value of $w_1$ is left unchanged. Remove card $2$. After this operation, $s = [2, 6, 2, 4, 4]$. </li><li> Select card $1$. Append $w_1 = 1$ to the end of $s$. Remove card $1$. After this operation, $s = [2, 6, 2, 4, 4, 1]$. </li></ol><p>One of the longest non-decreasing subsequences of $s = [2, 6, 2, 4, 4, 1]$ is $[2, 2, 4, 4]$. Thus, the length of the longest non-decreasing subsequence of $s$ is $4$. It can be proven that this is indeed the maximum possible length.</p>
