## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is a number of elements in the array</span>.</p><p>You are given an array $a$ consisting of $n$ integers. The value of the $i$-th element of the array is $a_i$.</p><p>You are also given a set of $m$ segments. The $j$-th segment is $[l_j; r_j]$, where $1 \le l_j \le r_j \le n$.</p><p>You can choose some subset of the given set of segments and decrease values on each of the chosen segments by one (<span class="tex-font-style-bf">independently</span>). For example, if the initial array $a = [0, 0, 0, 0, 0]$ and the given segments are $[1; 3]$ and $[2; 4]$ then you can choose both of them and the array will become $b = [-1, -2, -2, -1, 0]$.</p><p>You have to choose some subset of the given segments (<span class="tex-font-style-bf">each segment can be chosen at most once</span>) in such a way that if you apply this subset of segments to the array $a$ and obtain the array $b$ then the value $\max\limits_{i=1}^{n}b_i - \min\limits_{i=1}^{n}b_i$ will be <span class="tex-font-style-bf">maximum</span> possible.</p><p>Note that <span class="tex-font-style-bf">you can choose the empty set</span>.</p><p>If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p><p><span class="tex-font-style-bf">If you are Python programmer, consider using PyPy instead of Python when you submit your code.</span></p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($1 \le n \le 300, 0 \le m \le 300$) — the length of the array $a$ and the number of segments, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^6 \le a_i \le 10^6$), where $a_i$ is the value of the $i$-th element of the array $a$.</p><p>The next $m$ lines are contain two integers each. The $j$-th of them contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le n$), where $l_j$ and $r_j$ are the ends of the $j$-th segment.</p></div><div class="output-specification"><p>In the first line of the output print one integer $d$ — the <span class="tex-font-style-bf">maximum</span> possible value $\max\limits_{i=1}^{n}b_i - \min\limits_{i=1}^{n}b_i$ if $b$ is the array obtained by applying some subset of the given segments to the array $a$.</p><p>In the second line of the output print one integer $q$ ($0 \le q \le m$) — the number of segments you apply.</p><p>In the third line print $q$ distinct integers $c_1, c_2, \dots, c_q$ in <span class="tex-font-style-bf">any order</span> ($1 \le c_k \le m$) — indices of segments you apply to the array $a$ in such a way that the value $\max\limits_{i=1}^{n}b_i - \min\limits_{i=1}^{n}b_i$ of the obtained array $b$ is <span class="tex-font-style-bf">maximum</span> possible.</p><p>If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($1 \le n \le 300, 0 \le m \le 300$) — the length of the array $a$ and the number of segments, respectively.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^6 \le a_i \le 10^6$), where $a_i$ is the value of the $i$-th element of the array $a$.</p><p>The next $m$ lines are contain two integers each. The $j$-th of them contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le n$), where $l_j$ and $r_j$ are the ends of the $j$-th segment.</p>

## Output

<p>In the first line of the output print one integer $d$ — the <span class="tex-font-style-bf">maximum</span> possible value $\max\limits_{i=1}^{n}b_i - \min\limits_{i=1}^{n}b_i$ if $b$ is the array obtained by applying some subset of the given segments to the array $a$.</p><p>In the second line of the output print one integer $q$ ($0 \le q \le m$) — the number of segments you apply.</p><p>In the third line print $q$ distinct integers $c_1, c_2, \dots, c_q$ in <span class="tex-font-style-bf">any order</span> ($1 \le c_k \le m$) — indices of segments you apply to the array $a$ in such a way that the value $\max\limits_{i=1}^{n}b_i - \min\limits_{i=1}^{n}b_i$ of the obtained array $b$ is <span class="tex-font-style-bf">maximum</span> possible.</p><p>If there are multiple answers, you can print <span class="tex-font-style-bf">any</span>.</p>





```input1
5 4
2 -2 3 1 2
1 3
4 5
2 5
1 3
```




```input2
5 4
2 -2 3 1 4
3 5
3 4
2 4
2 5
```




```input3
1 0
1000000
```




```output1
6
2
1 4
```




```output2
7
2
3 2
```




```output3
0
0
```



## Note

<p>In the first example the obtained array $b$ will be $[0, -4, 1, 1, 2]$ so the answer is $6$.</p><p>In the second example the obtained array $b$ will be $[2, -3, 1, -1, 4]$ so the answer is $7$.</p><p>In the third example you cannot do anything so the answer is $0$.</p>
