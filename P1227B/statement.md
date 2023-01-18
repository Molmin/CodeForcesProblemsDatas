## Description

<div><p><span class="tex-font-style-it">Permutation</span> $p$ is a sequence of integers $p=[p_1, p_2, \dots, p_n]$, consisting of $n$ distinct (unique) positive integers between $1$ and $n$, inclusive. For example, the following sequences are permutations: $[3, 4, 1, 2]$, $[1]$, $[1, 2]$. The following sequences are not permutations: $[0]$, $[1, 2, 1]$, $[2, 3]$, $[0, 1, 2]$.</p><p>The important key is in the locked box that you need to open. To open the box you need to enter secret code. Secret code is a permutation $p$ of length $n$. </p><p>You don't know this permutation, you only know the array $q$ of prefix maximums of this permutation. Formally:</p><ul> <li> $q_1=p_1$, </li><li> $q_2=\max(p_1, p_2)$, </li><li> $q_3=\max(p_1, p_2,p_3)$, </li><li> ... </li><li> $q_n=\max(p_1, p_2,\dots,p_n)$. </li></ul><p>You want to construct any possible suitable permutation (i.e. any such permutation, that calculated $q$ for this permutation is equal to the given array).</p></div><div class="input-specification"><p>The first line contains integer number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of a test case contains one integer $n$ $(1 \le n \le 10^{5})$&nbsp;— the number of elements in the secret code permutation $p$.</p><p>The second line of a test case contains $n$ integers $q_1, q_2, \dots, q_n$ $(1 \le q_i \le n)$&nbsp;— elements of the array $q$ for secret permutation. It is guaranteed that $q_i \le q_{i+1}$ for all $i$ ($1 \le i &lt; n$).</p><p>The sum of all values $n$ over all the test cases in the input doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print:</p><ul> <li> If it's impossible to find such a permutation $p$, print "<span class="tex-font-style-tt">-1</span>" (without quotes). </li><li> Otherwise, print $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$). If there are multiple possible answers, you can print any of them. </li></ul></div>

## Input

<p>The first line contains integer number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of a test case contains one integer $n$ $(1 \le n \le 10^{5})$&nbsp;— the number of elements in the secret code permutation $p$.</p><p>The second line of a test case contains $n$ integers $q_1, q_2, \dots, q_n$ $(1 \le q_i \le n)$&nbsp;— elements of the array $q$ for secret permutation. It is guaranteed that $q_i \le q_{i+1}$ for all $i$ ($1 \le i &lt; n$).</p><p>The sum of all values $n$ over all the test cases in the input doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print:</p><ul> <li> If it's impossible to find such a permutation $p$, print "<span class="tex-font-style-tt">-1</span>" (without quotes). </li><li> Otherwise, print $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$). If there are multiple possible answers, you can print any of them. </li></ul>





```input1
4
5
1 3 4 5 5
4
1 1 3 4
2
2 2
1
1
```




```output1
1 3 4 5 2 
-1
2 1 
1
```



## Note

<p>In the first test case of the example answer $[1,3,4,5,2]$ is the only possible answer:</p><ul> <li> $q_{1} = p_{1} = 1$; </li><li> $q_{2} = \max(p_{1}, p_{2}) = 3$; </li><li> $q_{3} = \max(p_{1}, p_{2}, p_{3}) = 4$; </li><li> $q_{4} = \max(p_{1}, p_{2}, p_{3}, p_{4}) = 5$; </li><li> $q_{5} = \max(p_{1}, p_{2}, p_{3}, p_{4}, p_{5}) = 5$. </li></ul><p>It can be proved that there are no answers for the second test case of the example.</p>
