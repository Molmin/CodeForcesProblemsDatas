## Description

<div><p>For a permutation $p$ of numbers $1$ through $n$, we define a <span class="tex-font-style-it">stair array</span> $a$ as follows: $a_i$ is length of the longest segment of permutation which contains position $i$ and is made of consecutive values in sorted order: $[x, x+1, \ldots, y-1, y]$ or $[y, y-1, \ldots, x+1, x]$ for some $x \leq y$. For example, for permutation $p = [4, 1, 2, 3, 7, 6, 5]$ we have $a = [1, 3, 3, 3, 3, 3, 3]$. </p><p>You are given the stair array $a$. Your task is to calculate the number of permutations which have stair array equal to $a$. Since the number can be big, compute it modulo $998\,244\,353$. Note that this number can be equal to zero.</p></div><div class="input-specification"><p>The first line of input contains integer $n$ ($1 \le n \le 10^5$) &nbsp;— the length of a stair array $a$.</p><p>The second line of input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$).</p></div><div class="output-specification"><p>Print the number of permutations which have stair array equal to $a$. Since the number can be big, compute it modulo $998\,244\,353$.</p></div>

## Input

<p>The first line of input contains integer $n$ ($1 \le n \le 10^5$) &nbsp;— the length of a stair array $a$.</p><p>The second line of input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$).</p>

## Output

<p>Print the number of permutations which have stair array equal to $a$. Since the number can be big, compute it modulo $998\,244\,353$.</p>





```input1
6
3 3 3 1 1 1
```




```input2
7
4 4 4 4 3 3 3
```




```input3
1
1
```




```input4
8
2 2 2 2 2 2 1 1
```




```input5
4
3 2 3 1
```




```output1
6
```




```output2
6
```




```output3
1
```




```output4
370
```




```output5
0
```


