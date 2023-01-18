## Description

<div><p>Arkady invited Anna for a dinner to a sushi restaurant. The restaurant is a bit unusual: it offers $n$ pieces of sushi aligned in a row, and a customer has to choose a continuous subsegment of these sushi to buy.</p><p>The pieces of sushi are of two types: either with tuna or with eel. Let's denote the type of the $i$-th from the left sushi as $t_i$, where $t_i = 1$ means it is with tuna, and $t_i = 2$ means it is with eel.</p><p>Arkady does not like tuna, Anna does not like eel. Arkady wants to choose such a continuous subsegment of sushi that it has equal number of sushi of each type and each half of the subsegment has only sushi of one type. For example, subsegment $[2, 2, 2, 1, 1, 1]$ is valid, but subsegment $[1, 2, 1, 2, 1, 2]$ is not, because both halves contain both types of sushi.</p><p>Find the length of the longest continuous subsegment of sushi Arkady can buy.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 100\,000$)&nbsp;— the number of pieces of sushi.</p><p>The second line contains $n$ integers $t_1$, $t_2$, ..., $t_n$ ($t_i = 1$, denoting a sushi with tuna or $t_i = 2$, denoting a sushi with eel), representing the types of sushi from left to right.</p><p>It is guaranteed that there is at least one piece of sushi of each type. Note that it means that there is at least one valid continuous segment.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum length of a valid continuous segment.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 100\,000$)&nbsp;— the number of pieces of sushi.</p><p>The second line contains $n$ integers $t_1$, $t_2$, ..., $t_n$ ($t_i = 1$, denoting a sushi with tuna or $t_i = 2$, denoting a sushi with eel), representing the types of sushi from left to right.</p><p>It is guaranteed that there is at least one piece of sushi of each type. Note that it means that there is at least one valid continuous segment.</p>

## Output

<p>Print a single integer&nbsp;— the maximum length of a valid continuous segment.</p>





```input1
7
2 2 2 1 1 2 2
```




```input2
6
1 2 1 2 1 2
```




```input3
9
2 2 1 1 1 2 2 2 2
```




```output1
4
```




```output2
2
```




```output3
6
```



## Note

<p>In the first example Arkady can choose the subsegment $[2, 2, 1, 1]$ or the subsegment $[1, 1, 2, 2]$ with length $4$.</p><p>In the second example there is no way but to choose one of the subsegments $[2, 1]$ or $[1, 2]$ with length $2$.</p><p>In the third example Arkady's best choice is the subsegment $[1, 1, 1, 2, 2, 2]$.</p>
