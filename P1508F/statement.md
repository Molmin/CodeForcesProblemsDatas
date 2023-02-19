## Description

<div><p>Touko's favorite sequence of numbers is a permutation $a_1, a_2, \dots, a_n$ of $1, 2, \dots, n$, and she wants some collection of permutations that are similar to her favorite permutation.</p><p>She has a collection of $q$ intervals of the form $[l_i, r_i]$ with $1 \le l_i \le r_i \le n$. To create permutations that are similar to her favorite permutation, she coined the following definition:</p><ul> <li> A permutation $b_1, b_2, \dots, b_n$ allows an interval $[l', r']$ to <span class="tex-font-style-it">holds its shape</span> if for any pair of integers $(x, y)$ such that $l' \le x &lt; y \le r'$, we have $b_x &lt; b_y$ if and only if $a_x &lt; a_y$. </li><li> A permutation $b_1, b_2, \dots, b_n$ is <span class="tex-font-style-it">$k$-similar</span> if $b$ allows all intervals $[l_i, r_i]$ for all $1 \le i \le k$ to hold their shapes. </li></ul><p>Yuu wants to figure out all $k$-similar permutations for Touko, but it turns out this is a very hard task; instead, Yuu will <span class="tex-font-style-it">encode</span> the set of all $k$-similar permutations with directed acylic graphs (DAG). Yuu also coined the following definitions for herself:</p><ul> <li> A permutation $b_1, b_2, \dots, b_n$ <span class="tex-font-style-it">satisfies</span> a DAG $G'$ if for all edge $u \to v$ in $G'$, we must have $b_u &lt; b_v$. </li><li> A <span class="tex-font-style-it">$k$-encoding</span> is a DAG $G_k$ on the set of vertices $1, 2, \dots, n$ such that a permutation $b_1, b_2, \dots, b_n$ satisfies $G_k$ if and only if $b$ is $k$-similar. </li></ul><p>Since Yuu is free today, she wants to figure out the minimum number of edges among all $k$-encodings for each $k$ from $1$ to $q$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n \le 25\,000$, $1 \le q \le 100\,000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ which form a permutation of $1, 2, \dots, n$.</p><p>The $i$-th of the following $q$ lines contains two integers $l_i$ and $r_i$. ($1 \le l_i \le r_i \le n$).</p></div><div class="output-specification"><p>Print $q$ lines. The $k$-th of them should contain a single integer &nbsp;— The minimum number of edges among all $k$-encodings.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n \le 25\,000$, $1 \le q \le 100\,000$).</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ which form a permutation of $1, 2, \dots, n$.</p><p>The $i$-th of the following $q$ lines contains two integers $l_i$ and $r_i$. ($1 \le l_i \le r_i \le n$).</p>

## Output

<p>Print $q$ lines. The $k$-th of them should contain a single integer &nbsp;— The minimum number of edges among all $k$-encodings.</p>





```input1
4 3
2 4 1 3
1 3
2 4
1 4
```




```input2
8 4
3 7 4 8 1 5 2 6
3 6
1 6
3 8
1 8
```




```input3
10 10
10 5 1 2 7 3 9 4 6 8
2 2
4 5
6 8
4 10
4 4
2 7
2 2
7 8
3 7
2 10
```




```output1
2
4
3
```




```output2
3
5
9
7
```




```output3
0
1
3
6
6
9
9
9
9
8
```



## Note

<p>For the first test case:</p><ul><li> All $1$-similar permutations must allow the interval $[1, 3]$ to hold its shape. Therefore, the set of all $1$-similar permutations is $\{[3, 4, 2, 1], [3, 4, 1, 2], [2, 4, 1, 3], [2, 3, 1, 4]\}$. The optimal encoding of these permutations is<center> <img class="tex-graphics" src="file://z0vUGyTy.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li><li> All $2$-similar permutations must allow the intervals $[1, 3]$ and $[2, 4]$ to hold their shapes. Therefore, the set of all $2$-similar permutations is $\{[3, 4, 1, 2], [2, 4, 1, 3]\}$. The optimal encoding of these permutations is<center> <img class="tex-graphics" src="file://Uq5IIEmV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li><li> All $3$-similar permutations must allow the intervals $[1, 3]$, $[2, 4]$, and $[1, 4]$ to hold their shapes. Therefore, the set of all $3$-similar permutations only includes $[2, 4, 1, 3]$. The optimal encoding of this permutation is<center> <img class="tex-graphics" src="file://5BkMfW73.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></li></ul>
