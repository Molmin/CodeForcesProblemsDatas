## Description

<div><p><span class="tex-font-style-it">A bow adorned with nameless flowers that bears the earnest hopes of an equally nameless person.</span></p><p>You have obtained the elegant bow known as the Windblume Ode. Inscribed in the weapon is an array of $n$ ($n \ge 3$) positive <span class="tex-font-style-bf">distinct</span> integers (i.e. different, no duplicates are allowed).</p><p>Find the largest subset (i.e. having the maximum number of elements) of this array such that its sum is a composite number. A positive integer $x$ is called composite if there exists a positive integer $y$ such that $1 &lt; y &lt; x$ and $x$ is divisible by $y$.</p><p>If there are multiple subsets with this largest size with the composite sum, you can output any of them. It can be proven that under the constraints of the problem such a non-empty subset always exists.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 100$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_{1},a_{2},\dots,a_{n}$ ($1 \leq a_{i} \leq 200$)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Each test case should have two lines of output.</p><p>The first line should contain a single integer $x$: the size of the largest subset with composite sum. The next line should contain $x$ space separated integers representing the indices of the subset of the initial array.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ ($3 \leq n \leq 100$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ <span class="tex-font-style-bf">distinct</span> integers $a_{1},a_{2},\dots,a_{n}$ ($1 \leq a_{i} \leq 200$)&nbsp;— the elements of the array.</p>

## Output

<p>Each test case should have two lines of output.</p><p>The first line should contain a single integer $x$: the size of the largest subset with composite sum. The next line should contain $x$ space separated integers representing the indices of the subset of the initial array.</p>





```input1
4
3
8 1 2
4
6 9 4 2
9
1 2 3 4 5 6 7 8 9
3
200 199 198
```




```output1
2
2 1
4
2 1 4 3
9
6 9 1 2 3 4 5 7 8
3
1 2 3
```



## Note

<p>In the first test case, the subset $\{a_2, a_1\}$ has a sum of $9$, which is a composite number. The only subset of size $3$ has a prime sum equal to $11$. Note that you could also have selected the subset $\{a_1, a_3\}$ with sum $8 + 2 = 10$, which is composite as it's divisible by $2$.</p><p>In the second test case, the sum of all elements equals to $21$, which is a composite number. Here we simply take the whole array as our subset.</p>
