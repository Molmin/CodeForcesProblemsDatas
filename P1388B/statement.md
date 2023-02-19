## Description

<div><p><span class="tex-font-style-it">Captain Flint and his crew keep heading to a savage shore of Byteland for several months already, drinking rum and telling stories. In such moments uncle Bogdan often remembers his nephew Denis. Today, he has told a story about how Denis helped him to come up with an interesting problem and asked the crew to solve it.</span></p><p>In the beginning, uncle Bogdan wrote on a board a positive integer $x$ consisting of $n$ digits. After that, he wiped out $x$ and wrote integer $k$ instead, which was the concatenation of binary representations of digits $x$ consists of (without leading zeroes). For example, let $x = 729$, then $k = 111101001$ (since $7 = 111$, $2 = 10$, $9 = 1001$).</p><p>After some time, uncle Bogdan understood that he doesn't know what to do with $k$ and asked Denis to help. Denis decided to wipe last $n$ digits of $k$ and named the new number as $r$.</p><p>As a result, Denis proposed to find such integer $x$ of length $n$ that $r$ (as number) is maximum possible. If there are multiple valid $x$ then Denis is interested in the minimum one.</p><p>All crew members, including captain Flint himself, easily solved the task. All, except cabin boy Kostya, who was too drunk to think straight. But what about you?</p><p>Note: in this task, we compare integers ($x$ or $k$) as numbers (despite what representations they are written in), so $729 &lt; 1999$ or $111 &lt; 1000$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;— one per test case. The one and only line of each test case contains the single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the integer $x$ you need to find.</p><p>It's guaranteed that the sum of $n$ from all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print the minimum integer $x$ of length $n$ such that obtained by Denis number $r$ is maximum possible.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;— one per test case. The one and only line of each test case contains the single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the length of the integer $x$ you need to find.</p><p>It's guaranteed that the sum of $n$ from all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print the minimum integer $x$ of length $n$ such that obtained by Denis number $r$ is maximum possible.</p>





```input1
2
1
3
```




```output1
8
998
```



## Note

<p>In the second test case (with $n = 3$), if uncle Bogdan had $x = 998$ then $k = 100110011000$. Denis (by wiping last $n = 3$ digits) will obtain $r = 100110011$.</p><p>It can be proved that the $100110011$ is the maximum possible $r$ Denis can obtain and $998$ is the minimum $x$ to obtain it.</p>
