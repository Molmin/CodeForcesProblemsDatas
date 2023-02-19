## Description

<div><p>In winter, the inhabitants of the Moscow Zoo are very bored, in particular, it concerns gorillas. You decided to entertain them and brought a permutation $p$ of length $n$ to the zoo.</p><p>A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in any order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ occurs twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$, but $4$ is present in the array).</p><p>The gorillas had their own permutation $q$ of length $n$. They suggested that you count the number of pairs of integers $l, r$ ($1 \le l \le r \le n$) such that $\operatorname{MEX}([p_l, p_{l+1}, \ldots, p_r])=\operatorname{MEX}([q_l, q_{l+1}, \ldots, q_r])$.</p><p>The $\operatorname{MEX}$ of the sequence is the minimum integer <span class="tex-font-style-bf">positive</span> number missing from this sequence. For example, $\operatorname{MEX}([1, 3]) = 2$, $\operatorname{MEX}([5]) = 1$, $\operatorname{MEX}([3, 1, 2, 6]) = 4$.</p><p>You do not want to risk your health, so you will not dare to refuse the gorillas.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the permutations length.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$)&nbsp;— the elements of the permutation $p$.</p><p>The third line contains $n$ integers $q_1, q_2, \ldots, q_n$ ($1 \le q_i \le n$)&nbsp;— the elements of the permutation $q$.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of suitable pairs $l$ and $r$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the permutations length.</p><p>The second line contains $n$ integers $p_1, p_2, \ldots, p_n$ ($1 \le p_i \le n$)&nbsp;— the elements of the permutation $p$.</p><p>The third line contains $n$ integers $q_1, q_2, \ldots, q_n$ ($1 \le q_i \le n$)&nbsp;— the elements of the permutation $q$.</p>

## Output

<p>Print a single integer&nbsp;— the number of suitable pairs $l$ and $r$.</p>





```input1|
3
1 3 2
2 1 3
```




```input2|
7
7 3 6 2 1 5 4
6 7 2 5 3 1 4
```




```input3|
6
1 2 3 4 5 6
6 5 4 3 2 1
```




```output1
2
```




```output2
16
```




```output3
11
```



## Note

<p>In the first example, two segments are correct – $[1, 3]$ with $\operatorname{MEX}$ equal to $4$ in both arrays and $[3, 3]$ with $\operatorname{MEX}$ equal to $1$ in both of arrays.</p><p>In the second example, for example, the segment $[1, 4]$ is correct, and the segment $[6, 7]$ isn't correct, because $\operatorname{MEX}(5, 4) \neq \operatorname{MEX}(1, 4)$.</p>
