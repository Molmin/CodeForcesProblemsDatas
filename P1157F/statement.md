## Description

<div><p>There are $n$ people in a row. The height of the $i$-th person is $a_i$. You can choose <span class="tex-font-style-bf">any</span> subset of these people and try to arrange them into a <span class="tex-font-style-bf">balanced circle</span>.</p><p>A <span class="tex-font-style-bf">balanced circle</span> is such an order of people that the difference between heights of any adjacent people is no more than $1$. For example, let heights of chosen people be $[a_{i_1}, a_{i_2}, \dots, a_{i_k}]$, where $k$ is the number of people you choose. Then the condition $|a_{i_j} - a_{i_{j + 1}}| \le 1$ should be satisfied for all $j$ from $1$ to $k-1$ and the condition $|a_{i_1} - a_{i_k}| \le 1$ should be also satisfied. $|x|$ means the absolute value of $x$. It is obvious that the circle consisting of one person is balanced.</p><p>Your task is to choose the maximum number of people and construct a <span class="tex-font-style-bf">balanced circle</span> consisting of all chosen people. It is obvious that the circle consisting of one person is balanced so the answer always exists.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of people.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the height of the $i$-th person.</p></div><div class="output-specification"><p>In the first line of the output print $k$ — the number of people in the maximum <span class="tex-font-style-bf">balanced circle</span>.</p><p>In the second line print $k$ integers $res_1, res_2, \dots, res_k$, where $res_j$ is the <span class="tex-font-style-bf">height</span> of the $j$-th person in the maximum <span class="tex-font-style-bf">balanced circle</span>. The condition $|res_{j} - res_{j + 1}| \le 1$ should be satisfied for all $j$ from $1$ to $k-1$ and the condition $|res_{1} - res_{k}| \le 1$ should be also satisfied.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of people.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$), where $a_i$ is the height of the $i$-th person.</p>

## Output

<p>In the first line of the output print $k$ — the number of people in the maximum <span class="tex-font-style-bf">balanced circle</span>.</p><p>In the second line print $k$ integers $res_1, res_2, \dots, res_k$, where $res_j$ is the <span class="tex-font-style-bf">height</span> of the $j$-th person in the maximum <span class="tex-font-style-bf">balanced circle</span>. The condition $|res_{j} - res_{j + 1}| \le 1$ should be satisfied for all $j$ from $1$ to $k-1$ and the condition $|res_{1} - res_{k}| \le 1$ should be also satisfied.</p>





```input1
7
4 3 5 1 2 2 1
```




```input2
5
3 7 5 1 5
```




```input3
3
5 1 4
```




```input4
7
2 2 3 2 1 2 2
```




```output1
5
2 1 1 2 3
```




```output2
2
5 5
```




```output3
2
4 5
```




```output4
7
1 2 2 2 2 3 2
```


