## Description

<div><p>During the hypnosis session, Nicholas suddenly remembered a positive integer $n$, which <span class="tex-font-style-bf">doesn't contain zeros in decimal notation</span>. </p><p>Soon, when he returned home, he got curious: what is the maximum number of digits that can be removed from the number so that the number becomes <span class="tex-font-style-bf">not prime</span>, that is, either composite or equal to one?</p><p>For some numbers doing so is impossible: for example, for number $53$ it's impossible to delete some of its digits to obtain a not prime integer. However, <span class="tex-font-style-bf">for all $n$ in the test cases of this problem, it's guaranteed that it's possible to delete some of their digits to obtain a not prime number</span>.</p><p>Note that you cannot remove all the digits from the number.</p><p>A prime number is a number that has no divisors except one and itself. A composite is a number that has more than two divisors. $1$ is neither a prime nor a composite number.</p></div><div class="input-specification"><p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $k$ ($1 \le k \le 50$)&nbsp;— the number of digits in the number.</p><p>The second line of each test case contains a positive integer $n$, which doesn't contain zeros in decimal notation ($10^{k-1} \le n &lt; 10^{k}$). It is guaranteed that it is always possible to remove less than $k$ digits to make the number not prime.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>For every test case, print two numbers in two lines. In the first line print the number of digits, that you <span class="tex-font-style-bf">have left</span> in the number. In the second line print the digits left after all delitions. </p><p>If there are multiple solutions, print any.</p></div>

## Input

<p>Each test contains multiple test cases.</p><p>The first line contains one positive integer $t$ ($1 \le t \le 10^3$), denoting the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains one positive integer $k$ ($1 \le k \le 50$)&nbsp;— the number of digits in the number.</p><p>The second line of each test case contains a positive integer $n$, which doesn't contain zeros in decimal notation ($10^{k-1} \le n &lt; 10^{k}$). It is guaranteed that it is always possible to remove less than $k$ digits to make the number not prime.</p><p>It is guaranteed that the sum of $k$ over all test cases does not exceed $10^4$.</p>

## Output

<p>For every test case, print two numbers in two lines. In the first line print the number of digits, that you <span class="tex-font-style-bf">have left</span> in the number. In the second line print the digits left after all delitions. </p><p>If there are multiple solutions, print any.</p>





```input1
7
3
237
5
44444
3
221
2
35
3
773
1
4
30
626221626221626221626221626221
```




```output1
2
27
1
4
1
1
2
35
2
77
1
4
1
6
```



## Note

<p>In the first test case, you can't delete $2$ digits from the number $237$, as all the numbers $2$, $3$, and $7$ are prime. However, you can delete $1$ digit, obtaining a number $27 = 3^3$.</p><p>In the second test case, you can delete all digits except one, as $4 = 2^2$ is a composite number.</p>
