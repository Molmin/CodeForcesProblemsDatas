## Description

<div><p>You might have remembered Theatre square from the <a href="https://codeforces.com/problemset/problem/1/A">problem 1A</a>. Now it's finally getting repaved.</p><p>The square still has a rectangular shape of $n \times m$ meters. However, the picture is about to get more complicated now. Let $a_{i,j}$ be the $j$-th square in the $i$-th row of the pavement.</p><p>You are given the picture of the squares:</p><ul> <li> if $a_{i,j} = $ "<span class="tex-font-style-tt">*</span>", then the $j$-th square in the $i$-th row should be <span class="tex-font-style-bf">black</span>; </li><li> if $a_{i,j} = $ "<span class="tex-font-style-tt">.</span>", then the $j$-th square in the $i$-th row should be <span class="tex-font-style-bf">white</span>. </li></ul><p>The black squares are paved already. You have to pave the white squares. There are two options for pavement tiles:</p><ul> <li> $1 \times 1$ tiles&nbsp;— each tile costs $x$ burles and covers exactly $1$ square; </li><li> $1 \times 2$ tiles&nbsp;— each tile costs $y$ burles and covers exactly $2$ adjacent squares of the <span class="tex-font-style-bf">same row</span>. <span class="tex-font-style-bf">Note that you are not allowed to rotate these tiles or cut them into $1 \times 1$ tiles.</span> </li></ul><p><span class="tex-font-style-bf">You should cover all the white squares, no two tiles should overlap and no black squares should be covered by tiles.</span></p><p>What is the smallest total price of the tiles needed to cover all the white squares?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of testcases. Then the description of $t$ testcases follow.</p><p>The first line of each testcase contains four integers $n$, $m$, $x$ and $y$ ($1 \le n \le 100$; $1 \le m \le 1000$; $1 \le x, y \le 1000$)&nbsp;— the size of the Theatre square, the price of the $1 \times 1$ tile and the price of the $1 \times 2$ tile.</p><p>Each of the next $n$ lines contains $m$ characters. The $j$-th character in the $i$-th line is $a_{i,j}$. If $a_{i,j} = $ "<span class="tex-font-style-tt">*</span>", then the $j$-th square in the $i$-th row should be black, and if $a_{i,j} = $ "<span class="tex-font-style-tt">.</span>", then the $j$-th square in the $i$-th row should be white.</p><p><span class="tex-font-style-bf">It's guaranteed that the sum of $n \times m$ over all testcases doesn't exceed $10^5$.</span></p></div><div class="output-specification"><p>For each testcase print a single integer&nbsp;— the smallest total price of the tiles needed to cover all the white squares in burles.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 500$)&nbsp;— the number of testcases. Then the description of $t$ testcases follow.</p><p>The first line of each testcase contains four integers $n$, $m$, $x$ and $y$ ($1 \le n \le 100$; $1 \le m \le 1000$; $1 \le x, y \le 1000$)&nbsp;— the size of the Theatre square, the price of the $1 \times 1$ tile and the price of the $1 \times 2$ tile.</p><p>Each of the next $n$ lines contains $m$ characters. The $j$-th character in the $i$-th line is $a_{i,j}$. If $a_{i,j} = $ "<span class="tex-font-style-tt">*</span>", then the $j$-th square in the $i$-th row should be black, and if $a_{i,j} = $ "<span class="tex-font-style-tt">.</span>", then the $j$-th square in the $i$-th row should be white.</p><p><span class="tex-font-style-bf">It's guaranteed that the sum of $n \times m$ over all testcases doesn't exceed $10^5$.</span></p>

## Output

<p>For each testcase print a single integer&nbsp;— the smallest total price of the tiles needed to cover all the white squares in burles.</p>





```input1
4
1 1 10 1
.
1 2 10 1
..
2 1 10 1
.
.
3 3 3 7
..*
*..
.*.
```




```output1
10
1
20
18
```



## Note

<p>In the first testcase you are required to use a single $1 \times 1$ tile, even though $1 \times 2$ tile is cheaper. So the total price is $10$ burles.</p><p>In the second testcase you can either use two $1 \times 1$ tiles and spend $20$ burles or use a single $1 \times 2$ tile and spend $1$ burle. The second option is cheaper, thus the answer is $1$.</p><p>The third testcase shows that you can't rotate $1 \times 2$ tiles. You still have to use two $1 \times 1$ tiles for the total price of $20$.</p><p>In the fourth testcase the cheapest way is to use $1 \times 1$ tiles everywhere. The total cost is $6 \cdot 3 = 18$.</p>
