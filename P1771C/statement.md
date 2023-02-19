## Description

<div><p>Hossam has $n$ trainees. He assigned a number $a_i$ for the $i$-th trainee. </p><p>A pair of the $i$-th and $j$-th ($i \neq j$) trainees is called successful if there is an integer $x$ ($x \geq 2$), such that $x$ divides $a_i$, and $x$ divides $a_j$.</p><p>Hossam wants to know if there is a successful pair of trainees.</p><p>Hossam is very tired now, so he asks you for your help!</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$), the number of test cases. A description of the test cases follows.</p><p>The first line of each test case contains an integer number $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers, the number of each trainee $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>Print the answer —&nbsp;"<span class="tex-font-style-tt">YES</span>" (without quotes) if there is a successful pair of trainees and "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case.</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 10^5$), the number of test cases. A description of the test cases follows.</p><p>The first line of each test case contains an integer number $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers, the number of each trainee $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>Print the answer —&nbsp;"<span class="tex-font-style-tt">YES</span>" (without quotes) if there is a successful pair of trainees and "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each letter in any case.</p>





```input1|2,3
2
3
32 48 7
3
14 5 9
```




```output1
YES
NO
```



## Note

<p>In the first example, the first trainee and the second trainee make up a successful pair: </p><p>$a_1 = 32, a_2 = 48$, you can choose $x = 4$.</p>
