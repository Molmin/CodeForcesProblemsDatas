## Description

<div><p>Another Codeforces Round has just finished! It has gathered $n$ participants, and according to the results, the expected rating change of participant $i$ is $a_i$. These rating changes are <span class="tex-font-style-it">perfectly balanced</span>&nbsp;— their sum is equal to $0$.</p><p>Unfortunately, due to minor technical glitches, the round is declared <span class="tex-font-style-it">semi-rated</span>. It means that all rating changes must be divided by two.</p><p>There are two conditions though: </p><ul> <li> For each participant $i$, their modified rating change $b_i$ must be integer, and as close to $\frac{a_i}{2}$ as possible. It means that either $b_i = \lfloor \frac{a_i}{2} \rfloor$ or $b_i = \lceil \frac{a_i}{2} \rceil$. In particular, if $a_i$ is even, $b_i = \frac{a_i}{2}$. Here $\lfloor x \rfloor$ denotes rounding down to the largest integer not greater than $x$, and $\lceil x \rceil$ denotes rounding up to the smallest integer not smaller than $x$. </li><li> The modified rating changes must be perfectly balanced&nbsp;— their sum must be equal to $0$. </li></ul><p>Can you help with that?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 13\,845$), denoting the number of participants.</p><p>Each of the next $n$ lines contains a single integer $a_i$ ($-336 \le a_i \le 1164$), denoting the rating change of the $i$-th participant.</p><p>The sum of all $a_i$ is equal to $0$.</p></div><div class="output-specification"><p>Output $n$ integers $b_i$, each denoting the modified rating change of the $i$-th participant in order of input.</p><p>For any $i$, it must be true that either $b_i = \lfloor \frac{a_i}{2} \rfloor$ or $b_i = \lceil \frac{a_i}{2} \rceil$. The sum of all $b_i$ must be equal to $0$.</p><p>If there are multiple solutions, print any. We can show that a solution exists for any valid input.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 13\,845$), denoting the number of participants.</p><p>Each of the next $n$ lines contains a single integer $a_i$ ($-336 \le a_i \le 1164$), denoting the rating change of the $i$-th participant.</p><p>The sum of all $a_i$ is equal to $0$.</p>

## Output

<p>Output $n$ integers $b_i$, each denoting the modified rating change of the $i$-th participant in order of input.</p><p>For any $i$, it must be true that either $b_i = \lfloor \frac{a_i}{2} \rfloor$ or $b_i = \lceil \frac{a_i}{2} \rceil$. The sum of all $b_i$ must be equal to $0$.</p><p>If there are multiple solutions, print any. We can show that a solution exists for any valid input.</p>





```input1
3
10
-5
-5
```




```input2
7
-7
-29
0
3
24
-29
38
```




```output1
5
-2
-3
```




```output2
-3
-15
0
2
12
-15
19
```



## Note

<p>In the first example, $b_1 = 5$, $b_2 = -3$ and $b_3 = -2$ is another correct solution.</p><p>In the second example there are $6$ possible solutions, one of them is shown in the example output.</p>
