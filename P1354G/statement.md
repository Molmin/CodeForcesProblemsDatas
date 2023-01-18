## Description

<div><p><span class="tex-font-style-it">This is an interactive problem. Don't forget to flush output after printing queries using <span class="tex-font-style-tt">cout.flush()</span> or <span class="tex-font-style-tt">fflush(stdout)</span> in <span class="tex-font-style-tt">C++</span> or similar functions in other programming languages.</span></p><p>There are $n$ gift boxes in a row, numbered from $1$ to $n$ from left to right. It's known that exactly $k$ of them contain valuable gifts&nbsp;— other boxes contain just lucky stones. All boxes look the same and differ only in weight. All <span class="tex-font-style-it">boxes with stones have the same weight and are strictly heavier</span> than boxes with valuable items. But valuable gifts may be different, so the boxes with valuable items may have different weights.</p><p>You can ask no more than $50$ queries (printing an answer doesn't count). By each query you can compare total weights of two non-intersecting subsets of boxes $a_1, a_2, \dots, a_{k_a}$ and $b_1, b_2, \dots, b_{k_b}$. In return you'll get one of four results:</p><ul> <li> <span class="tex-font-style-tt">FIRST</span>, if subset $a_1, a_2, \dots, a_{k_a}$ is strictly <span class="tex-font-style-bf">heavier</span>; </li><li> <span class="tex-font-style-tt">SECOND</span>, if subset $b_1, b_2, \dots, b_{k_b}$ is strictly <span class="tex-font-style-bf">heavier</span>; </li><li> <span class="tex-font-style-tt">EQUAL</span>, if subsets have equal total weights; </li><li> <span class="tex-font-style-tt">WASTED</span>, if the query is incorrect or the limit of queries is exceeded. </li></ul><p>Using such queries (or, maybe, intuition) find the box with a valuable gift with <span class="tex-font-style-bf">the minimum index</span>.</p></div><div class="input-specification"><p>The input consists of several cases. In the beginning, you receive the integer $T$ ($1 \le T \le 500$)&nbsp;— the number of test cases.</p><p>At the beginning of each test case, you receive two integers $n$ and $k$ ($2 \le n \le 1000$, $1 \le k \le \frac{n}{2}$)&nbsp;— the number of boxes in a row and the number of boxes with valuable gifts.</p><p>It's guaranteed that the order of boxes is fixed beforehand and that the sum of $n$ in one test doesn't exceed $1000$.</p></div><div class="output-specification"><p>For each test case print the minimum index among all boxes with a valuable gift in the following format: "<span class="tex-font-style-tt">! $x$</span>" where $x$ ($1 \le x \le n$)&nbsp;— the index of the box.</p></div><div><h2>Interaction</h2><p>Print each query in three lines. In the first line print the sizes of subset in the following format: "<span class="tex-font-style-tt">? $k_a$ $k_b$</span>" where $k_a$ and $k_b$ ($1 \le k_a, k_b \le n$; $k_a + k_b \le n$)&nbsp;— the corresponding sizes.</p><p>In the second line print $k_a$ integers $a_1, a_2, \dots, a_{k_a}$ ($1 \le a_i \le n$; $a_i \neq a_j$ if $i \neq j$)&nbsp;— indexes of boxes in the first subset.</p><p>In the third line print $k_b$ integers $b_1, b_2, \dots, b_{k_b}$ ($1 \le b_i \le n$; $b_i \neq b_j$ if $i \neq j$)&nbsp;— indexes of boxes in the second subset.</p><p>The subsets shouldn't intersect, i. e. $a_i \neq b_j$ for all $i$ and $j$.</p><p>You'll receive one of four responses described above. In the case of <span class="tex-font-style-tt">WASTED</span> stop your program to avoid getting random verdict instead of <span class="tex-font-style-tt">Wrong Answer</span>.</p></div>

## Input

<p>The input consists of several cases. In the beginning, you receive the integer $T$ ($1 \le T \le 500$)&nbsp;— the number of test cases.</p><p>At the beginning of each test case, you receive two integers $n$ and $k$ ($2 \le n \le 1000$, $1 \le k \le \frac{n}{2}$)&nbsp;— the number of boxes in a row and the number of boxes with valuable gifts.</p><p>It's guaranteed that the order of boxes is fixed beforehand and that the sum of $n$ in one test doesn't exceed $1000$.</p>

## Output

<p>For each test case print the minimum index among all boxes with a valuable gift in the following format: "<span class="tex-font-style-tt">! $x$</span>" where $x$ ($1 \le x \le n$)&nbsp;— the index of the box.</p>





```input1
2
2 1
-
-
-
FIRST
-
5 2
-
-
-
FIRST
-
-
-
SECOND
-
-
-
EQUAL
-
```




```output1
-
-
? 1 1
1
2
-
! 2
-
? 1 1
1
2
-
? 2 3
4 2
1 3 5
-
? 1 1
4
5
-
! 1
```



## Note

<p>Additional separators "–" in the sample are used only to increase the readability of the sample. <span class="tex-font-style-bf">Don't print any unnecessary symbols or line breaks in your solution when you send it to the system.</span></p><p><span class="tex-font-style-it">Hacks are forbidden in this task.</span></p>
