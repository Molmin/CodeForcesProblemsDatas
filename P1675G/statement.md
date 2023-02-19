## Description

<div><p>Nastya baked $m$ pancakes and spread them on $n$ dishes. The dishes are in a row and numbered from left to right. She put $a_i$ pancakes on the dish with the index $i$.</p><p>Seeing the dishes, Vlad decided to bring order to the stacks and move some pancakes. In one move, he can shift one pancake from any dish to the closest one, that is, select the dish $i$ ($a_i &gt; 0$) and do one of the following:</p><ul><li> if $i &gt; 1$, put the pancake on a dish with the previous index, after this move $a_i = a_i - 1$ and $a_{i - 1} = a_{i - 1} + 1$;</li><li> if $i &lt; n$, put the pancake on a dish with the following index, after this move $a_i = a_i - 1$ and $a_{i + 1} = a_{i + 1} + 1$.</li></ul><p>Vlad wants to make the array $a$<span class="tex-font-style-bf">non-increasing</span>, after moving as few pancakes as possible. Help him find the minimum number of moves needed for this.</p><p>The array $a=[a_1, a_2,\dots,a_n]$ is called non-increasing if $a_i \ge a_{i+1}$ for all $i$ from $1$ to $n-1$.</p></div><div class="input-specification"><p>The first line of the input contains two numbers $n$ and $m$ ($1 \le n, m \le 250$) — the number of dishes and the number of pancakes, respectively.</p><p>The second line contains $n$ numbers $a_i$ ($0 \le a_i \le m$), the sum of all $a_i$ is equal to $m$.</p></div><div class="output-specification"><p>Print a single number: the minimum number of moves required to make the array $a$ non-increasing.</p></div>

## Input

<p>The first line of the input contains two numbers $n$ and $m$ ($1 \le n, m \le 250$) — the number of dishes and the number of pancakes, respectively.</p><p>The second line contains $n$ numbers $a_i$ ($0 \le a_i \le m$), the sum of all $a_i$ is equal to $m$.</p>

## Output

<p>Print a single number: the minimum number of moves required to make the array $a$ non-increasing.</p>





```input1
6 19
5 3 2 3 3 3
```




```input2
3 6
3 2 1
```




```input3
3 6
2 1 3
```




```input4
6 19
3 4 3 3 5 1
```




```input5
10 1
0 0 0 0 0 0 0 0 0 1
```




```output1
2
```




```output2
0
```




```output3
1
```




```output4
3
```




```output5
9
```



## Note

<p>In the first example, you first need to move the pancake from the dish $1$, after which $a = [4, 4, 2, 3, 3, 3]$. After that, you need to move the pancake from the dish $2$ to the dish $3$ and the array will become non-growing $a = [4, 3, 3, 3, 3, 3]$.</p>
