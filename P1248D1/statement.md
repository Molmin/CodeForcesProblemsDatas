## Description

<div><p>This is an easier version of the problem. In this version, $n \le 500$.</p><p>Vasya is an experienced developer of programming competitions' problems. As all great minds at some time, Vasya faced a creative crisis. To improve the situation, Petya gifted him a string consisting of opening and closing brackets only. Petya believes, that the beauty of the bracket string is a number of its cyclical shifts, which form a correct bracket sequence.</p><p>To digress from his problems, Vasya decided to select two positions of the string (<span class="tex-font-style-bf">not necessarily distinct</span>) and swap characters located at this positions with each other. Vasya will apply this operation exactly once. He is curious what is the maximum possible beauty he can achieve this way. Please help him.</p><p>We remind that bracket sequence $s$ is called correct if: </p><ul> <li> $s$ is empty; </li><li> $s$ is equal to "<span class="tex-font-style-tt">(</span>$t$<span class="tex-font-style-tt">)</span>", where $t$ is correct bracket sequence; </li><li> $s$ is equal to $t_1 t_2$, i.e. concatenation of $t_1$ and $t_2$, where $t_1$ and $t_2$ are correct bracket sequences. </li></ul><p>For example, "<span class="tex-font-style-tt">(()())</span>", "<span class="tex-font-style-tt">()</span>" are correct, while "<span class="tex-font-style-tt">)(</span>" and "<span class="tex-font-style-tt">())</span>" are not.</p><p>The cyclical shift of the string $s$ of length $n$ by $k$ ($0 \leq k &lt; n$) is a string formed by a concatenation of the last $k$ symbols of the string $s$ with the first $n - k$ symbols of string $s$. For example, the cyclical shift of string "<span class="tex-font-style-tt">(())()</span>" by $2$ equals "<span class="tex-font-style-tt">()(())</span>".</p><p>Cyclical shifts $i$ and $j$ are considered different, if $i \ne j$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 500$), the length of the string.</p><p>The second line contains a string, consisting of exactly $n$ characters, where each of the characters is either "<span class="tex-font-style-tt">(</span>" or "<span class="tex-font-style-tt">)</span>".</p></div><div class="output-specification"><p>The first line should contain a single integer&nbsp;— the largest beauty of the string, which can be achieved by swapping some two characters.</p><p>The second line should contain integers $l$ and $r$ ($1 \leq l, r \leq n$)&nbsp;— the indices of two characters, which should be swapped in order to maximize the string's beauty.</p><p>In case there are several possible swaps, print any of them.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 500$), the length of the string.</p><p>The second line contains a string, consisting of exactly $n$ characters, where each of the characters is either "<span class="tex-font-style-tt">(</span>" or "<span class="tex-font-style-tt">)</span>".</p>

## Output

<p>The first line should contain a single integer&nbsp;— the largest beauty of the string, which can be achieved by swapping some two characters.</p><p>The second line should contain integers $l$ and $r$ ($1 \leq l, r \leq n$)&nbsp;— the indices of two characters, which should be swapped in order to maximize the string's beauty.</p><p>In case there are several possible swaps, print any of them.</p>





```input1
10
()()())(()
```




```input2
12
)(()(()())()
```




```input3
6
)))(()
```




```output1
5
8 7
```




```output2
4
5 10
```




```output3
0
1 1
```



## Note

<p>In the first example, we can swap $7$-th and $8$-th character, obtaining a string "<span class="tex-font-style-tt">()()()()()</span>". The cyclical shifts by $0, 2, 4, 6, 8$ of this string form a correct bracket sequence.</p><p>In the second example, after swapping $5$-th and $10$-th character, we obtain a string "<span class="tex-font-style-tt">)(())()()(()</span>". The cyclical shifts by $11, 7, 5, 3$ of this string form a correct bracket sequence.</p><p>In the third example, swap of any two brackets results in $0$ cyclical shifts being correct bracket sequences. </p>
