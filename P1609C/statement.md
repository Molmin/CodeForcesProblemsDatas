## Description

<div><center> <img class="tex-graphics" height="302px" src="file://mzW1wmca.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>While performing complex market analysis William encountered the following problem:</p><p>For a given array $a$ of size $n$ and a natural number $e$, calculate the number of pairs of natural numbers $(i, k)$ which satisfy the following conditions: </p><ul> <li> $1 \le i, k$ </li><li> $i + e \cdot k \le n$. </li><li> Product $a_i \cdot a_{i + e} \cdot a_{i + 2 \cdot e} \cdot \ldots \cdot a_{i + k \cdot e} $ is a prime number. </li></ul><p>A prime number (or a prime) is a natural number greater than 1 that is not a product of two smaller natural numbers.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $e$ $(1 \le e \le n \le 2 \cdot 10^5)$, the number of items in the array and number $e$, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^6)$, the contents of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case output the answer in the following format:</p><p>Output one line containing the number of pairs of numbers $(i, k)$ which satisfy the conditions.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $e$ $(1 \le e \le n \le 2 \cdot 10^5)$, the number of items in the array and number $e$, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i \le 10^6)$, the contents of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case output the answer in the following format:</p><p>Output one line containing the number of pairs of numbers $(i, k)$ which satisfy the conditions.</p>





```input1
6
7 3
10 2 1 3 1 19 3
3 2
1 13 1
9 3
2 4 2 1 1 1 1 4 2
3 1
1 1 1
4 1
1 2 1 1
2 2
1 2
```




```output1
2
0
4
0
5
0
```



## Note

<p>In the first example test case two pairs satisfy the conditions: </p><ol> <li> $i = 2, k = 1$, for which the product is: $a_{2} \cdot a_{5} = 2$ which is a prime number. </li><li> $i = 3, k = 1$, for which the product is: $a_{3} \cdot a_{6} = 19$ which is a prime number. </li></ol><p>In the second example test case there are no pairs that satisfy the conditions.</p><p>In the third example test case four pairs satisfy the conditions: </p><ol> <li> $i = 1, k = 1$, for which the product is: $a_{1} \cdot a_{4} = 2$ which is a prime number. </li><li> $i = 1, k = 2$, for which the product is: $a_{1} \cdot a_{4} \cdot a_{7} = 2$ which is a prime number. </li><li> $i = 3, k = 1$, for which the product is: $a_{3} \cdot a_{6} = 2$ which is a prime number. </li><li> $i = 6, k = 1$, for which the product is: $a_{6} \cdot a_{9} = 2$ which is a prime number. </li></ol><p>In the fourth example test case there are no pairs that satisfy the conditions.</p><p>In the fifth example test case five pairs satisfy the conditions: </p><ol> <li> $i = 1, k = 1$, for which the product is: $a_{1} \cdot a_{2} = 2$ which is a prime number. </li><li> $i = 1, k = 2$, for which the product is: $a_{1} \cdot a_{2} \cdot a_{3} = 2$ which is a prime number. </li><li> $i = 1, k = 3$, for which the product is: $a_{1} \cdot a_{2} \cdot a_{3} \cdot a_{4} = 2$ which is a prime number. </li><li> $i = 2, k = 1$, for which the product is: $a_{2} \cdot a_{3} = 2$ which is a prime number. </li><li> $i = 2, k = 2$, for which the product is: $a_{2} \cdot a_{3} \cdot a_{4} = 2$ which is a prime number. </li></ol><p>In the sixth example test case there are no pairs that satisfy the conditions.</p>
