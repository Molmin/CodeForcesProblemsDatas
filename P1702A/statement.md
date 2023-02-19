## Description

<div><p>At the store, the salespeople want to make all prices <span class="tex-font-style-it">round</span>. </p><p>In this problem, a number that is a power of $10$ is called a <span class="tex-font-style-it">round</span> number. For example, the numbers $10^0 = 1$, $10^1 = 10$, $10^2 = 100$ are <span class="tex-font-style-it">round</span> numbers, but $20$, $110$ and $256$ are not <span class="tex-font-style-it">round</span> numbers. </p><p>So, if an item is worth $m$ bourles (the value of the item is not greater than $10^9$), the sellers want to change its value to the nearest <span class="tex-font-style-it">round</span> number that is not greater than $m$. They ask you: by how many bourles should you <span class="tex-font-style-bf">decrease</span> the value of the item to make it worth exactly $10^k$ bourles, where the value of $k$&nbsp;— is the maximum possible ($k$&nbsp;— any non-negative integer).</p><p>For example, let the item have a value of $178$-bourles. Then the new price of the item will be $100$, and the answer will be $178-100=78$.</p></div><div class="input-specification"><p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases .</p><p>Each test case is a string containing a single integer $m$ ($1 \le m \le 10^9$)&nbsp;— the price of the item.</p></div><div class="output-specification"><p>For each test case, output on a separate line a single integer $d$ ($0 \le d &lt; m$) such that if you reduce the cost of the item by $d$ bourles, the cost of the item will be the maximal possible <span class="tex-font-style-it">round</span> number. More formally: $m - d = 10^k$, where $k$&nbsp;— the maximum possible non-negative integer.</p></div>

## Input

<p>The first line of input data contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases .</p><p>Each test case is a string containing a single integer $m$ ($1 \le m \le 10^9$)&nbsp;— the price of the item.</p>

## Output

<p>For each test case, output on a separate line a single integer $d$ ($0 \le d &lt; m$) such that if you reduce the cost of the item by $d$ bourles, the cost of the item will be the maximal possible <span class="tex-font-style-it">round</span> number. More formally: $m - d = 10^k$, where $k$&nbsp;— the maximum possible non-negative integer.</p>





```input1|2,4,6,8
7
1
2
178
20
999999999
9000
987654321
```




```output1
0
1
78
10
899999999
8000
887654321
```



## Note

<p>In the example:</p><ul> <li> $1 - 0 = 10^0$, </li><li> $2 - 1 = 10^0$, </li><li> $178 - 78 = 10^2$, </li><li> $20 - 10 = 10^1$, </li><li> $999999999 - 899999999 = 10^8$, </li><li> $9000 - 8000 = 10^3$, </li><li> $987654321 - 887654321 = 10^8$. </li></ul><p>Note that in each test case, we get the maximum possible <span class="tex-font-style-it">round</span> number.</p>
