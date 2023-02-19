## Description

<div><p>A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array) and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>Let $p$ be any permutation of length $n$. We define the <span class="tex-font-style-bf">fingerprint</span> $F(p)$ of $p$ as the sorted array of sums of adjacent elements in $p$. More formally,</p><p>$$F(p)=\mathrm{sort}([p_1+p_2,p_2+p_3,\ldots,p_{n-1}+p_n]).$$</p><p>For example, if $n=4$ and $p=[1,4,2,3],$ then the fingerprint is given by $F(p)=\mathrm{sort}([1+4,4+2,2+3])=\mathrm{sort}([5,6,5])=[5,5,6]$.</p><p>You are given a permutation $p$ of length $n$. Your task is to find a <span class="tex-font-style-bf">different</span> permutation $p'$ with the same fingerprint. Two permutations $p$ and $p'$ are considered different if there is some index $i$ such that $p_i \ne p'_i$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 668$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 100$) &nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1,\ldots,p_n$ ($1\le p_i\le n$). It is guaranteed that $p$ is a permutation.</p></div><div class="output-specification"><p>For each test case, output $n$ integers $p'_1,\ldots, p'_n$ — a permutation such that $p'\ne p$ and $F(p')=F(p)$.</p><p>We can prove that for every permutation satisfying the input constraints, a solution exists.</p><p>If there are multiple solutions, you may output any.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 668$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($2\le n\le 100$) &nbsp;— the length of the permutation.</p><p>The second line of each test case contains $n$ integers $p_1,\ldots,p_n$ ($1\le p_i\le n$). It is guaranteed that $p$ is a permutation.</p>

## Output

<p>For each test case, output $n$ integers $p'_1,\ldots, p'_n$ — a permutation such that $p'\ne p$ and $F(p')=F(p)$.</p><p>We can prove that for every permutation satisfying the input constraints, a solution exists.</p><p>If there are multiple solutions, you may output any.</p>





```input1
3
2
1 2
6
2 1 6 5 4 3
5
2 4 3 1 5
```




```output1
2 1
1 2 5 6 3 4
3 1 5 2 4
```



## Note

<p>In the first test case, $F(p)=\mathrm{sort}([1+2])=[3]$.</p><p>And $F(p')=\mathrm{sort}([2+1])=[3]$.</p><p>In the second test case, $F(p)=\mathrm{sort}([2+1,1+6,6+5,5+4,4+3])=\mathrm{sort}([3,7,11,9,7])=[3,7,7,9,11]$.</p><p>And $F(p')=\mathrm{sort}([1+2,2+5,5+6,6+3,3+4])=\mathrm{sort}([3,7,11,9,7])=[3,7,7,9,11]$.</p><p>In the third test case, $F(p)=\mathrm{sort}([2+4,4+3,3+1,1+5])=\mathrm{sort}([6,7,4,6])=[4,6,6,7]$.</p><p>And $F(p')=\mathrm{sort}([3+1,1+5,5+2,2+4])=\mathrm{sort}([4,6,7,6])=[4,6,6,7]$.</p>
