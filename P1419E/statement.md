## Description

<div><p>An agent called Cypher is decrypting a message, that contains a <a href="https://en.wikipedia.org/wiki/Composite_number">composite number</a> $n$. All divisors of $n$, which are greater than $1$, are placed in a circle. Cypher can choose the initial order of numbers in the circle.</p><p>In one move Cypher can choose two adjacent numbers in a circle and insert their <a href="https://en.wikipedia.org/wiki/Least_common_multiple">least common multiple</a> between them. He can do that move as many times as needed.</p><p>A message is decrypted, if every two adjacent numbers are not coprime. Note that for such constraints it's always possible to decrypt the message.</p><p>Find the minimal number of moves that Cypher should do to decrypt the message, and show the initial order of numbers in the circle for that.</p></div><div class="input-specification"><p>The first line contains an integer $t$ $(1 \le t \le 100)$&nbsp;— the number of test cases. Next $t$ lines describe each test case.</p><p>In a single line of each test case description, there is a single composite number $n$ $(4 \le n \le 10^9)$&nbsp;— the number from the message.</p><p>It's guaranteed that the total number of divisors of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case in the first line output the initial order of divisors, which are greater than $1$, in the circle. In the second line output, the minimal number of moves needed to decrypt the message.</p><p>If there are different possible orders with a correct answer, print any of them.</p></div>

## Input

<p>The first line contains an integer $t$ $(1 \le t \le 100)$&nbsp;— the number of test cases. Next $t$ lines describe each test case.</p><p>In a single line of each test case description, there is a single composite number $n$ $(4 \le n \le 10^9)$&nbsp;— the number from the message.</p><p>It's guaranteed that the total number of divisors of $n$ for all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case in the first line output the initial order of divisors, which are greater than $1$, in the circle. In the second line output, the minimal number of moves needed to decrypt the message.</p><p>If there are different possible orders with a correct answer, print any of them.</p>





```input1
3
6
4
30
```




```output1
2 3 6 
1
2 4 
0
2 30 6 3 15 5 10 
0
```



## Note

<p>In the first test case $6$ has three divisors, which are greater than $1$: $2, 3, 6$. Regardless of the initial order, numbers $2$ and $3$ are adjacent, so it's needed to place their least common multiple between them. After that the circle becomes $2, 6, 3, 6$, and every two adjacent numbers are not coprime.</p><p>In the second test case $4$ has two divisors greater than $1$: $2, 4$, and they are not coprime, so any initial order is correct, and it's not needed to place any least common multiples.</p><p>In the third test case all divisors of $30$ greater than $1$ can be placed in some order so that there are no two adjacent numbers that are coprime.</p>
