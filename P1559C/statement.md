## Description

<div><p>The city where Mocha lives in is called Zhijiang. There are $n+1$ villages and $2n-1$ directed roads in this city. </p><p>There are two kinds of roads:</p><ul> <li> $n-1$ roads are from village $i$ to village $i+1$, for all $1\leq i \leq n-1$. </li><li> $n$ roads can be described by a sequence $a_1,\ldots,a_n$. If $a_i=0$, the $i$-th of these roads goes from village $i$ to village $n+1$, otherwise it goes from village $n+1$ to village $i$, for all $1\leq i\leq n$. </li></ul><p>Mocha plans to go hiking with Taki this weekend. To avoid the trip being boring, they plan to go through every village <span class="tex-font-style-bf">exactly once</span>. They can start and finish at any villages. Can you help them to draw up a plan? </p></div><div class="input-specification"><p>Each test contains multiple test cases. </p><p>The first line contains a single integer $t$ ($1 \le t \le 20$) — the number of test cases. Each test case consists of two lines.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^4$) — indicates that the number of villages is $n+1$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$). If $a_i=0$, it means that there is a road from village $i$ to village $n+1$. If $a_i=1$, it means that there is a road from village $n+1$ to village $i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p></div><div class="output-specification"><p>For each test case, print a line with $n+1$ integers, where the $i$-th number is the $i$-th village they will go through. If the answer doesn't exist, print $-1$.</p><p>If there are multiple correct answers, you can print any one of them.</p></div>

## Input

<p>Each test contains multiple test cases. </p><p>The first line contains a single integer $t$ ($1 \le t \le 20$) — the number of test cases. Each test case consists of two lines.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^4$) — indicates that the number of villages is $n+1$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$). If $a_i=0$, it means that there is a road from village $i$ to village $n+1$. If $a_i=1$, it means that there is a road from village $n+1$ to village $i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^4$.</p>

## Output

<p>For each test case, print a line with $n+1$ integers, where the $i$-th number is the $i$-th village they will go through. If the answer doesn't exist, print $-1$.</p><p>If there are multiple correct answers, you can print any one of them.</p>





```input1
2
3
0 1 0
3
1 1 0
```




```output1
1 4 2 3 
4 1 2 3
```



## Note

<p>In the first test case, the city looks like the following graph:</p><p><img class="tex-graphics" src="file://M4WtE81n.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>So all possible answers are $(1 \to 4 \to 2 \to 3)$, $(1 \to 2 \to 3 \to 4)$.</p><p>In the second test case, the city looks like the following graph:</p><p><img class="tex-graphics" src="file://mOpTELHO.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>So all possible answers are $(4 \to 1 \to 2 \to 3)$, $(1 \to 2 \to 3 \to 4)$, $(3 \to 4 \to 1 \to 2)$, $(2 \to 3 \to 4 \to 1)$.</p>
