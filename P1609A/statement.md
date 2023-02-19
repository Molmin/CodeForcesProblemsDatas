## Description

<div><center> <img class="tex-graphics" height="302px" src="file://80gVMdFa.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>William has array of $n$ numbers $a_1, a_2, \dots, a_n$. He can perform the following sequence of operations <span class="tex-font-style-bf">any number of times</span>: </p><ol> <li> Pick any two items from array $a_i$ and $a_j$, where $a_i$ must be a multiple of $2$ </li><li> $a_i = \frac{a_i}{2}$ </li><li> $a_j = a_j \cdot 2$ </li></ol><p>Help William find the maximal sum of array elements, which he can get by performing the sequence of operations described above.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ $(1 \le n \le 15)$, the number of elements in William's array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i &lt; 16)$, the contents of William's array.</p></div><div class="output-specification"><p>For each test case output the maximal sum of array elements after performing an optimal sequence of operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The first line of each test case contains an integer $n$ $(1 \le n \le 15)$, the number of elements in William's array.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ $(1 \le a_i &lt; 16)$, the contents of William's array.</p>

## Output

<p>For each test case output the maximal sum of array elements after performing an optimal sequence of operations.</p>





```input1
5
3
6 4 2
5
1 2 3 4 5
1
10
3
2 3 4
15
8 8 8 8 8 8 8 8 8 8 8 8 8 8 8
```




```output1
50
46
10
26
35184372088846
```



## Note

<p>In the first example test case the optimal sequence would be: </p><ol> <li> Pick $i = 2$ and $j = 1$. After performing a sequence of operations $a_2 = \frac{4}{2} = 2$ and $a_1 = 6 \cdot 2 = 12$, making the array look as: [12, 2, 2]. </li><li> Pick $i = 2$ and $j = 1$. After performing a sequence of operations $a_2 = \frac{2}{2} = 1$ and $a_1 = 12 \cdot 2 = 24$, making the array look as: [24, 1, 2]. </li><li> Pick $i = 3$ and $j = 1$. After performing a sequence of operations $a_3 = \frac{2}{2} = 1$ and $a_1 = 24 \cdot 2 = 48$, making the array look as: [48, 1, 1]. </li></ol><p>The final answer $48 + 1 + 1 = 50$.</p><p>In the third example test case there is no way to change the sum of elements, so the answer is $10$.</p>
