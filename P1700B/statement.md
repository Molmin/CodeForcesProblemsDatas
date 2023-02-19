## Description

<div><p>During a daily walk Alina noticed a long number written on the ground. Now Alina wants to find some positive number of same length without leading zeroes, such that the sum of these two numbers is a palindrome. </p><p>Recall that a number is called a palindrome, if it reads the same right to left and left to right. For example, numbers $121, 66, 98989$ are palindromes, and $103, 239, 1241$ are not palindromes.</p><p>Alina understands that a valid number always exist. Help her find one!</p></div><div class="input-specification"><p>The first line of input data contains an integer $t$ ($1 \leq t \leq 100$) — the number of test cases. Next, descriptions of $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 100\,000$) — the length of the number that is written on the ground.</p><p>The second line of contains the positive $n$-digit integer without leading zeroes — the number itself.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $100\,000$.</p></div><div class="output-specification"><p>For each of $t$ test cases print an answer — a positive $n$-digit integer without leading zeros, such that the sum of the input integer and this number is a palindrome.</p><p>We can show that at least one number satisfying the constraints exists. If there are multiple solutions, you can output any of them.</p></div>

## Input

<p>The first line of input data contains an integer $t$ ($1 \leq t \leq 100$) — the number of test cases. Next, descriptions of $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($2 \leq n \leq 100\,000$) — the length of the number that is written on the ground.</p><p>The second line of contains the positive $n$-digit integer without leading zeroes — the number itself.</p><p>It is guaranteed that the sum of the values $n$ over all test cases does not exceed $100\,000$.</p>

## Output

<p>For each of $t$ test cases print an answer — a positive $n$-digit integer without leading zeros, such that the sum of the input integer and this number is a palindrome.</p><p>We can show that at least one number satisfying the constraints exists. If there are multiple solutions, you can output any of them.</p>





```input1
3
2
99
4
1023
3
385
```




```output1
32
8646
604
```



## Note

<p>In the first test case $99 + 32 = 131$ is a palindrome. Note that another answer is $12$, because $99 + 12 = 111$ is also a palindrome.</p><p>In the second test case $1023 + 8646 = 9669$.</p><p>In the third test case $385 + 604 = 989$.</p>
