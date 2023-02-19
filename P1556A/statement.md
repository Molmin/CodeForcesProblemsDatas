## Description

<div><center> <img class="tex-graphics" height="302px" src="file://TnpVeAQf.png" style="max-width: 100.0%;max-height: 100.0%;" width="454px"> </center><p>William has two numbers $a$ and $b$ initially both equal to <span class="tex-font-style-bf">zero</span>. William mastered performing three different operations with them quickly. Before performing each operation some positive integer $k$ is picked, which is then used to perform one of the following operations: (note, that for each operation you can choose a <span class="tex-font-style-bf">new</span> positive integer $k$)</p><ol> <li> add number $k$ to both $a$ and $b$, or </li><li> add number $k$ to $a$ and subtract $k$ from $b$, or </li><li> add number $k$ to $b$ and subtract $k$ from $a$. </li></ol><p>Note that after performing operations, numbers $a$ and $b$ may become negative as well.</p><p>William wants to find out the minimal number of operations he would have to perform to make $a$ equal to his favorite number $c$ and $b$ equal to his second favorite number $d$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The only line of each test case contains two integers $c$ and $d$ $(0 \le c, d \le 10^9)$, which are William's favorite numbers and which he wants $a$ and $b$ to be transformed into.</p></div><div class="output-specification"><p>For each test case output a single number, which is the minimal number of operations which William would have to perform to make $a$ equal to $c$ and $b$ equal to $d$, or $-1$ if it is impossible to achieve this using the described operations.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). Description of the test cases follows.</p><p>The only line of each test case contains two integers $c$ and $d$ $(0 \le c, d \le 10^9)$, which are William's favorite numbers and which he wants $a$ and $b$ to be transformed into.</p>

## Output

<p>For each test case output a single number, which is the minimal number of operations which William would have to perform to make $a$ equal to $c$ and $b$ equal to $d$, or $-1$ if it is impossible to achieve this using the described operations.</p>





```input1
6
1 2
3 5
5 3
6 6
8 0
0 0
```




```output1
-1
2
2
1
2
0
```



## Note

<p>Let us demonstrate one of the suboptimal ways of getting a pair $(3, 5)$:</p><ul> <li> Using an operation of the first type with $k=1$, the current pair would be equal to $(1, 1)$. </li><li> Using an operation of the third type with $k=8$, the current pair would be equal to $(-7, 9)$. </li><li> Using an operation of the second type with $k=7$, the current pair would be equal to $(0, 2)$. </li><li> Using an operation of the first type with $k=3$, the current pair would be equal to $(3, 5)$. </li></ul>
