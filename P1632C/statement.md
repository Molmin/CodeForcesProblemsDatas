## Description

<div><p>Igor is in 11th grade. Tomorrow he will have to write an informatics test by the strictest teacher in the school, Pavel Denisovich. </p><p>Igor knows how the test will be conducted: first of all, the teacher will give each student two positive integers $a$ and $b$ ($a &lt; b$). After that, the student can apply any of the following operations any number of times: </p><ul> <li> $a := a + 1$ (increase $a$ by $1$), </li><li> $b := b + 1$ (increase $b$ by $1$), </li><li> $a := a \ | \ b$ (replace $a$ with the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> of $a$ and $b$). </li></ul><p>To get full marks on the test, the student has to tell the teacher the minimum required number of operations to make $a$ and $b$ equal.</p><p>Igor already knows which numbers the teacher will give him. Help him figure out what is the minimum number of operations needed to make $a$ equal to $b$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The only line for each test case contains two integers $a$ and $b$ ($1 \le a &lt; b \le 10^6$).</p><p><span class="tex-font-style-bf">It is guaranteed that the sum of $b$ over all test cases does not exceed $10^6$.</span></p></div><div class="output-specification"><p>For each test case print one integer — the minimum required number of operations to make $a$ and $b$ equal.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The only line for each test case contains two integers $a$ and $b$ ($1 \le a &lt; b \le 10^6$).</p><p><span class="tex-font-style-bf">It is guaranteed that the sum of $b$ over all test cases does not exceed $10^6$.</span></p>

## Output

<p>For each test case print one integer — the minimum required number of operations to make $a$ and $b$ equal.</p>





```input1
5
1 3
5 8
2 5
3 19
56678 164422
```




```output1
1
3
2
1
23329
```



## Note

<p>In the first test case, it is optimal to apply the third operation.</p><p>In the second test case, it is optimal to apply the first operation three times.</p><p>In the third test case, it is optimal to apply the second operation and then the third operation.</p>
