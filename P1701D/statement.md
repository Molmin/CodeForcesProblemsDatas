## Description

<div><p>Monocarp had a permutation $a$ of $n$ integers $1$, $2$, ..., $n$ (a permutation is an array where each element from $1$ to $n$ occurs exactly once).</p><p>Then Monocarp calculated an array of integers $b$ of size $n$, where $b_i = \left\lfloor \frac{i}{a_i} \right\rfloor$. For example, if the permutation $a$ is $[2, 1, 4, 3]$, then the array $b$ is equal to $\left[ \left\lfloor \frac{1}{2} \right\rfloor, \left\lfloor \frac{2}{1} \right\rfloor, \left\lfloor \frac{3}{4} \right\rfloor, \left\lfloor \frac{4}{3} \right\rfloor \right] = [0, 2, 0, 1]$.</p><p>Unfortunately, the Monocarp has lost his permutation, so he wants to restore it. Your task is to find a permutation $a$ that corresponds to the given array $b$. If there are multiple possible permutations, then print any of them. The tests are constructed in such a way that least one suitable permutation exists.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i \le n$).</p><p>Additional constrains on the input:</p><ul> <li> the sum of $n$ over test cases does not exceed $5 \cdot 10^5$; </li><li> there exists at least one permutation $a$ that would yield this array $b$. </li></ul></div><div class="output-specification"><p>For each test case, print $n$ integers&nbsp;— a permutation $a$ that corresponds to the given array $b$. If there are multiple possible permutations, then print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^5$)&nbsp;— number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 5 \cdot 10^5$).</p><p>The second line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i \le n$).</p><p>Additional constrains on the input:</p><ul> <li> the sum of $n$ over test cases does not exceed $5 \cdot 10^5$; </li><li> there exists at least one permutation $a$ that would yield this array $b$. </li></ul>

## Output

<p>For each test case, print $n$ integers&nbsp;— a permutation $a$ that corresponds to the given array $b$. If there are multiple possible permutations, then print any of them.</p>





```input1|2,3,6,7
4
4
0 2 0 1
2
1 1
5
0 0 1 4 1
3
0 1 3
```




```output1
2 1 4 3 
1 2 
3 4 2 1 5 
3 2 1
```


