## Description

<div><p>You are given an array of integers $a_1, a_2, \ldots, a_n$ and an integer $x$.</p><p>You need to select the maximum number of elements in the array, such that for every subsegment $a_l, a_{l + 1}, \ldots, a_r$ containing strictly more than one element $(l &lt; r)$, either: </p><ul> <li> At least one element on this subsegment is <span class="tex-font-style-bf">not</span> selected, or </li><li> $a_l + a_{l+1} + \ldots + a_r \geq x \cdot (r - l + 1)$. </li></ul></div><div class="input-specification"><p>The first line of input contains one integer $t$ ($1 \leq t \leq 10$): the number of test cases.</p><p>The descriptions of $t$ test cases follow, three lines per test case.</p><p>In the first line you are given one integer $n$ ($1 \leq n \leq 50\,000$): the number of integers in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-100\,000 \leq a_i \leq 100\,000$).</p><p>The third line contains one integer $x$ ($-100\,000 \leq x \leq 100\,000$).</p></div><div class="output-specification"><p>For each test case, print one integer: the maximum number of elements that you can select.</p></div>

## Input

<p>The first line of input contains one integer $t$ ($1 \leq t \leq 10$): the number of test cases.</p><p>The descriptions of $t$ test cases follow, three lines per test case.</p><p>In the first line you are given one integer $n$ ($1 \leq n \leq 50\,000$): the number of integers in the array.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-100\,000 \leq a_i \leq 100\,000$).</p><p>The third line contains one integer $x$ ($-100\,000 \leq x \leq 100\,000$).</p>

## Output

<p>For each test case, print one integer: the maximum number of elements that you can select.</p>





```input1
4
5
1 2 3 4 5
2
10
2 4 2 4 2 4 2 4 2 4
3
3
-10 -5 -10
-8
3
9 9 -3
5
```




```output1
4
8
2
2
```



## Note

<p>In the first example, one valid way to select the elements is $[\underline{1}, 2, \underline{3}, \underline{4}, \underline{5}]$. All subsegments satisfy at least one of the criteria. For example, for the subsegment $l = 1$, $r = 2$ we have that the element $2$ is not selected, satisfying the first criterion. For the subsegment $l = 3$, $r = 5$ we have $3 + 4 + 5 = 12 \ge 2 \cdot 3$, satisfying the second criterion.</p><p>We can't select all elements, because in this case for $l = 1$, $r = 2$ all elements are selected and we have $a_1 + a_2 = 3 &lt; 2 \cdot 2$. Thus, the maximum number of selected elements is $4$.</p><p>In the second example, one valid solution is $[\underline{2}, \underline{4}, 2, \underline{4}, \underline{2}, \underline{4}, 2, \underline{4}, \underline{2}, \underline{4}]$.</p><p>In the third example, one valid solution is $[\underline{-10}, -5, \underline{-10}]$.</p><p>In the fourth example, one valid solution is $[\underline{9}, \underline{9}, -3]$.</p>
