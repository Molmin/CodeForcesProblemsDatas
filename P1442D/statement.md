## Description

<div><p>You are given $n$ <span class="tex-font-style-bf">non-decreasing</span> arrays of non-negative numbers. </p><p>Vasya repeats the following operation $k$ times: </p><ul> <li> Selects a non-empty array. </li><li> Puts the first element of the selected array in his pocket. </li><li> Removes the first element from the selected array. </li></ul><p>Vasya wants to maximize the sum of the elements in his pocket.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n, k \le 3\,000$): the number of arrays and operations.</p><p>Each of the next $n$ lines contain an array. The first integer in each line is $t_i$ ($1 \le t_i \le 10^6$): the size of the $i$-th array. The following $t_i$ integers $a_{i, j}$ ($0 \le a_{i, 1} \le \ldots \le a_{i, t_i} \le 10^8$) are the elements of the $i$-th array.</p><p>It is guaranteed that $k \le \sum\limits_{i=1}^n t_i \le 10^6$.</p></div><div class="output-specification"><p>Print one integer: the maximum possible sum of all elements in Vasya's pocket after $k$ operations.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n, k \le 3\,000$): the number of arrays and operations.</p><p>Each of the next $n$ lines contain an array. The first integer in each line is $t_i$ ($1 \le t_i \le 10^6$): the size of the $i$-th array. The following $t_i$ integers $a_{i, j}$ ($0 \le a_{i, 1} \le \ldots \le a_{i, t_i} \le 10^8$) are the elements of the $i$-th array.</p><p>It is guaranteed that $k \le \sum\limits_{i=1}^n t_i \le 10^6$.</p>

## Output

<p>Print one integer: the maximum possible sum of all elements in Vasya's pocket after $k$ operations.</p>





```input1
3 3
2 5 10
3 1 2 3
2 1 20
```




```output1
26
```


