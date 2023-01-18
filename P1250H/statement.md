## Description

<div><p>You have a set of birthday cake candles. Each of such candles represents a digit between $0$ and $9$, inclusive.</p><center> <img class="tex-graphics" src="file://6RIu0qHT.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Example of birthday cake candles.</span> </center><p>Let's denote the candle representing the digit $d$ as $d$-candle.</p><p>Your set contains $c_0$ instances of $0$-candles, $c_1$ instances of $1$-candles and so on. So, the total number of candles is $c_0+c_1+\dots+c_9$.</p><p>These digits are needed to wish your cat a happy birthday. For each birthday, starting with the first, you want to compose the age of the cat using the digits from the set.</p><p>Since you light candles for a very short time, candles don't have time to burn out. For this reason <span class="tex-font-style-it">you can reuse candles an arbitrary number of times</span> (therefore your set of candles never changes).</p><p>For example, if you have one instance of each digit (i.e. $c_0=c_1=\dots=c_9=1$), you can compose any number from $1$ to $10$ using this set, but you cannot compose $11$.</p><p>You have to determine the first birthday, on which you cannot compose the age of the cat using the candles from your set. In other words, find the minimum number $y$ such that all numbers from $1$ to $y-1$ can be composed by digits from your set, but $y$ cannot be composed.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input.</p><p>The only line of each test case contains ten integer numbers $c_0, c_1, \dots, c_9$ ($0 \le c_i \le 10^5$) — the number of $0$-candles, $1$-candles, $2$-candles and so on.</p><p>It is guaranteed that the sum of all $c_i$ in the input does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case, output one integer in single line — the minimum age which cannot be composed by candles from your set. Please note that the age can be quite large (it may exceed the standard 64-bit integer types in your programming language).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input.</p><p>The only line of each test case contains ten integer numbers $c_0, c_1, \dots, c_9$ ($0 \le c_i \le 10^5$) — the number of $0$-candles, $1$-candles, $2$-candles and so on.</p><p>It is guaranteed that the sum of all $c_i$ in the input does not exceed $10^6$.</p>

## Output

<p>For each test case, output one integer in single line — the minimum age which cannot be composed by candles from your set. Please note that the age can be quite large (it may exceed the standard 64-bit integer types in your programming language).</p>





```input1
4
1 1 1 1 1 1 1 1 1 1
0 0 1 1 2 2 3 3 4 4
1 2 1 2 1 3 1 0 0 0
0 1 2 1 4 3 1 1 2 1
```




```output1
11
1
7
10
```


