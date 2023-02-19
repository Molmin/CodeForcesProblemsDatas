## Description

<div><p>Given an array $a$ of $n$ elements, print any value that appears at least three times or print <span class="tex-font-style-tt">-1</span> if there is no such value.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p></div><div class="output-specification"><p>For each test case, print any value that appears at least three times or print <span class="tex-font-style-tt">-1</span> if there is no such value.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 2\cdot10^5$)&nbsp;— the length of the array.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i \leq n$)&nbsp;— the elements of the array.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2\cdot10^5$.</p>

## Output

<p>For each test case, print any value that appears at least three times or print <span class="tex-font-style-tt">-1</span> if there is no such value.</p>





```input1
7
1
1
3
2 2 2
7
2 2 3 3 4 2 2
8
1 4 3 4 3 2 4 1
9
1 1 1 2 2 2 3 3 3
5
1 5 2 4 3
4
4 4 4 4
```




```output1
-1
2
2
4
3
-1
4
```



## Note

<p>In the first test case there is just a single element, so it can't occur at least three times and the answer is <span class="tex-font-style-tt">-1</span>.</p><p>In the second test case, all three elements of the array are equal to $2$, so $2$ occurs three times, and so the answer is $2$.</p><p>For the third test case, $2$ occurs four times, so the answer is $2$.</p><p>For the fourth test case, $4$ occurs three times, so the answer is $4$.</p><p>For the fifth test case, $1$, $2$ and $3$ all occur at least three times, so they are all valid outputs.</p><p>For the sixth test case, all elements are distinct, so none of them occurs at least three times and the answer is <span class="tex-font-style-tt">-1</span>.</p>
