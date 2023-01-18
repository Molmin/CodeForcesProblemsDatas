## Description

<div><p>We guessed a permutation $p$ consisting of $n$ integers. The permutation of length $n$ is the array of length $n$ where each element from $1$ to $n$ appears exactly once. This permutation is a secret for you.</p><p>For each position $r$ from $2$ to $n$ we chose some other index $l$ ($l &lt; r$) and gave you the segment $p_l, p_{l + 1}, \dots, p_r$ in <span class="tex-font-style-bf">sorted</span> order (i.e. we rearranged the elements of this segment in a way that the elements of this segment are sorted). Thus, you are given exactly $n-1$ segments of the initial permutation but elements inside each segment are sorted. The segments are given to you in random order.</p><p>For example, if the secret permutation is $p=[3, 1, 4, 6, 2, 5]$ then the possible given set of segments can be:</p><ul> <li> $[2, 5, 6]$ </li><li> $[4, 6]$ </li><li> $[1, 3, 4]$ </li><li> $[1, 3]$ </li><li> $[1, 2, 4, 6]$ </li></ul><p>Your task is to find <span class="tex-font-style-bf">any</span> suitable permutation (i.e. any permutation corresponding to the given input data). It is guaranteed that the input data corresponds to some permutation (i.e. such permutation exists).</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 200$) — the length of the permutation.</p><p>The next $n-1$ lines describe given segments.</p><p>The $i$-th line contains the description of the $i$-th segment. The line starts with the integer $k_i$ ($2 \le k_i \le n$) — the length of the $i$-th segment. Then $k_i$ integers follow. All integers in a line are distinct, sorted in ascending order, between $1$ and $n$, inclusive.</p><p>It is guaranteed that the required $p$ exists for each test case.</p><p>It is also guaranteed that the sum of $n$ over all test cases does not exceed $200$ ($\sum n \le 200$).</p></div><div class="output-specification"><p>For each test case, print the answer: $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$, all $p_i$ should be distinct) — <span class="tex-font-style-bf">any</span> suitable permutation (i.e. any permutation corresponding to the test case input).</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 100$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains one integer $n$ ($2 \le n \le 200$) — the length of the permutation.</p><p>The next $n-1$ lines describe given segments.</p><p>The $i$-th line contains the description of the $i$-th segment. The line starts with the integer $k_i$ ($2 \le k_i \le n$) — the length of the $i$-th segment. Then $k_i$ integers follow. All integers in a line are distinct, sorted in ascending order, between $1$ and $n$, inclusive.</p><p>It is guaranteed that the required $p$ exists for each test case.</p><p>It is also guaranteed that the sum of $n$ over all test cases does not exceed $200$ ($\sum n \le 200$).</p>

## Output

<p>For each test case, print the answer: $n$ integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$, all $p_i$ should be distinct) — <span class="tex-font-style-bf">any</span> suitable permutation (i.e. any permutation corresponding to the test case input).</p>





```input1
5
6
3 2 5 6
2 4 6
3 1 3 4
2 1 3
4 1 2 4 6
5
2 2 3
2 1 2
2 1 4
2 4 5
7
3 1 2 6
4 1 3 5 6
2 1 2
3 4 5 7
6 1 2 3 4 5 6
3 1 3 6
2
2 1 2
5
2 2 5
3 2 3 5
4 2 3 4 5
5 1 2 3 4 5
```




```output1
3 1 4 6 2 5 
3 2 1 4 5 
2 1 6 3 5 4 7 
1 2 
2 5 3 4 1
```


