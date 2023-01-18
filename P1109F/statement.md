## Description

<div><p>One fine day Sasha went to the park for a walk. In the park, he saw that his favorite bench is occupied, and he had to sit down on the neighboring one. He sat down and began to listen to the silence. Suddenly, he got a question: what if in different parts of the park, the silence sounds in different ways? So it was. Let's divide the park into $1 \times 1$ meter squares and call them <span class="tex-font-style-it">cells</span>, and numerate rows from $1$ to $n$ from up to down, and columns from $1$ to $m$ from left to right. And now, every cell can be described with a pair of two integers $(x, y)$, where $x$&nbsp;— the number of the row, and $y$&nbsp;— the number of the column. Sasha knows that the level of silence in the cell $(i, j)$ equals to $f_{i,j}$, and all $f_{i,j}$ form a permutation of numbers from $1$ to $n \cdot m$. Sasha decided to count, how many are there <span class="tex-font-style-it">pleasant</span> segments of silence?</p><p>Let's take some segment $[l \ldots r]$. Denote $S$ as the set of cells $(i, j)$ that $l \le f_{i,j} \le r$. Then, the segment of silence $[l \ldots r]$ is <span class="tex-font-style-it">pleasant</span> if there is only <span class="tex-font-style-bf">one simple</span> path between every pair of cells from $S$ (path can't contain cells, which are not in $S$). In other words, set $S$ should look like a tree on a plain. Sasha has done this task pretty quickly, and called the algorithm&nbsp;— "algorithm of silence's sounds".</p><p>Time passed, and the only thing left from the algorithm is a legend. To prove the truthfulness of this story, you have to help Sasha and to find the number of <span class="tex-font-style-bf">different</span> <span class="tex-font-style-it">pleasant</span> segments of silence. Two segments $[l_1 \ldots r_1]$, $[l_2 \ldots r_2]$ are different, if $l_1 \neq l_2$ or $r_1 \neq r_2$ or both at the same time.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 1000$, $1 \le n \cdot m \le 2 \cdot 10^5$)&nbsp;— the size of the park.</p><p>Each from next $n$ lines contains $m$ integers $f_{i,j}$ ($1 \le f_{i,j} \le n \cdot m$)&nbsp;— the level of silence in the cell with number $(i, j)$.</p><p>It is guaranteed, that all $f_{i,j}$ are different.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">pleasant</span> segments of silence.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 1000$, $1 \le n \cdot m \le 2 \cdot 10^5$)&nbsp;— the size of the park.</p><p>Each from next $n$ lines contains $m$ integers $f_{i,j}$ ($1 \le f_{i,j} \le n \cdot m$)&nbsp;— the level of silence in the cell with number $(i, j)$.</p><p>It is guaranteed, that all $f_{i,j}$ are different.</p>

## Output

<p>Print one integer&nbsp;— the number of <span class="tex-font-style-it">pleasant</span> segments of silence.</p>





```input1
1 5
1 2 3 4 5

```




```input2
2 3
1 2 3
4 5 6

```




```input3
4 4
4 3 2 16
1 13 14 15
5 7 8 12
6 11 9 10

```




```output1
15
```




```output2
15
```




```output3
50
```



## Note

<p>In the first example, all segments of silence are <span class="tex-font-style-it">pleasant</span>.</p><p>In the second example, <span class="tex-font-style-it">pleasant</span> segments of silence are the following:</p><p><img class="tex-graphics" src="file://0T2pH6vi.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
