## Description

<div><p>There is a classroom with two rows of computers. There are $n$ computers in each row and each computer has its own grade. Computers in the first row has grades $a_1, a_2, \dots, a_n$ and in the second row&nbsp;— $b_1, b_2, \dots, b_n$.</p><p>Initially, all pairs of <span class="tex-font-style-bf">neighboring</span> computers in each row are connected by wire (pairs $(i, i + 1)$ for all $1 \le i &lt; n$), so two rows form two independent computer networks.</p><p>Your task is to combine them in one common network by connecting one or more pairs of computers from <span class="tex-font-style-bf">different</span> rows. Connecting the $i$-th computer from the first row and the $j$-th computer from the second row costs $|a_i - b_j|$.</p><p>You can connect one computer to several other computers, but you need to provide at least a basic fault tolerance: you need to connect computers in such a way that the network stays connected, despite one of its computer failing. In other words, if one computer is broken (no matter which one), the network won't split in two or more parts.</p><p>That is the minimum total cost to make a fault-tolerant network?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains the single integer $n$ ($3 \le n \le 2 \cdot 10^5$)&nbsp;— the number of computers in each row.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the grades of computers in the first row.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the grades of computers in the second row.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the minimum total cost to make a fault-tolerant network.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. Next $t$ cases follow.</p><p>The first line of each test case contains the single integer $n$ ($3 \le n \le 2 \cdot 10^5$)&nbsp;— the number of computers in each row.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the grades of computers in the first row.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the grades of computers in the second row.</p><p>It's guaranteed that the total sum of $n$ doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the minimum total cost to make a fault-tolerant network.</p>





```input1
2
3
1 10 1
20 4 25
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000
```




```output1
31
1999999998
```



## Note

<p>In the first test case, it's optimal to connect four pairs of computers: </p><ol> <li> computer $1$ from the first row with computer $2$ from the second row: cost $|1 - 4| = 3$; </li><li> computer $3$ from the first row with computer $2$ from the second row: cost $|1 - 4| = 3$; </li><li> computer $2$ from the first row with computer $1$ from the second row: cost $|10 - 20| = 10$; </li><li> computer $2$ from the first row with computer $3$ from the second row: cost $|10 - 25| = 15$; </li></ol> In total, $3 + 3 + 10 + 15 = 31$.<p>In the second test case, it's optimal to connect $1$ from the first row with $1$ from the second row, and $4$ from the first row with $4$ from the second row.</p>
