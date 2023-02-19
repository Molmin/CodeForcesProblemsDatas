## Description

<div><p>Petya has got an interesting flower. Petya is a busy person, so he sometimes forgets to water it. You are given $n$ days from Petya's live and you have to determine what happened with his flower in the end.</p><p>The flower grows as follows: </p><ul> <li> If the flower isn't watered for two days in a row, it dies. </li><li> If the flower is watered in the $i$-th day, it grows by $1$ centimeter. </li><li> If the flower is watered in the $i$-th and in the $(i-1)$-th day ($i &gt; 1$), then it grows by $5$ centimeters instead of $1$. </li><li> If the flower is not watered in the $i$-th day, it does not grow. </li></ul><p>At the beginning of the $1$-st day the flower is $1$ centimeter tall. What is its height after $n$ days?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains the only integer $n$ ($1 \leq n \leq 100$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($a_i = 0$ or $a_i = 1$). If $a_i = 1$, the flower is watered in the $i$-th day, otherwise it is not watered.</p></div><div class="output-specification"><p>For each test case print a single integer $k$ — the flower's height after $n$ days, or $-1$, if the flower dies.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). Description of the test cases follows.</p><p>The first line of each test case contains the only integer $n$ ($1 \leq n \leq 100$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($a_i = 0$ or $a_i = 1$). If $a_i = 1$, the flower is watered in the $i$-th day, otherwise it is not watered.</p>

## Output

<p>For each test case print a single integer $k$ — the flower's height after $n$ days, or $-1$, if the flower dies.</p>





```input1
4
3
1 0 1
3
0 1 1
4
1 0 0 1
1
0
```




```output1
3
7
-1
1
```


