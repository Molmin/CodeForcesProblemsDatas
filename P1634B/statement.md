## Description

<div><div class="epigraph"><div class="epigraph-text">Haha, try to solve this, SelectorUnlimited!</div><div class="epigraph-source">— antontrygubO_o</div></div><p>Your friends Alice and Bob practice fortune telling.</p><p>Fortune telling is performed as follows. There is a well-known array $a$ of $n$ non-negative integers indexed from $1$ to $n$. The tellee starts with some non-negative number $d$ and performs one of the two operations for each $i = 1, 2, \ldots, n$, <span class="tex-font-style-bf">in the increasing order of $i$</span>. The possible operations are:</p><ul><li> replace their current number $d$ with $d + a_i$</li><li> replace their current number $d$ with $d \oplus a_i$ (hereinafter $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Exclusive_or">bitwise XOR operation</a>)</li></ul><p>Notice that the chosen operation may be different for different $i$ and for different tellees.</p><p>One time, Alice decided to start with $d = x$ and Bob started with $d = x + 3$. Each of them performed fortune telling and got a particular number in the end. Notice that the friends chose operations independently of each other, that is, they could apply different operations for the same $i$.</p><p>You learnt that either Alice or Bob ended up with number $y$ in the end, but you don't know whose of the two it was. Given the numbers Alice and Bob started with and $y$, find out who (Alice or Bob) could get the number $y$ after performing the operations. It is guaranteed that on the jury tests, <span class="tex-font-style-bf">exactly one</span> of your friends could have actually gotten that number.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>You cannot make hacks in this problem.</p></div><div class="input-specification"><p>On the first line of the input, you are given one number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The following $2 \cdot t$ lines contain test cases.</p><p>The first line of each test case contains three numbers $n$, $x$, $y$ ($1 \le n \le 10^5$, $0 \le x \le 10^9$, $0 \le y \le 10^{15}$)&nbsp;— the length of array $a$, Alice's initial number (Bob's initial number is therefore $x+3$), and the number that one of the two friends got in the end.</p><p>The second line of each test case contains $n$ numbers&nbsp;— the array $a$ ($0 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print the name of the friend who could get the number $y$: "Alice" or "Bob".</p></div>

## Input

<p>On the first line of the input, you are given one number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The following $2 \cdot t$ lines contain test cases.</p><p>The first line of each test case contains three numbers $n$, $x$, $y$ ($1 \le n \le 10^5$, $0 \le x \le 10^9$, $0 \le y \le 10^{15}$)&nbsp;— the length of array $a$, Alice's initial number (Bob's initial number is therefore $x+3$), and the number that one of the two friends got in the end.</p><p>The second line of each test case contains $n$ numbers&nbsp;— the array $a$ ($0 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print the name of the friend who could get the number $y$: "Alice" or "Bob".</p>





```input1|2,3,6,7
4
1 7 9
2
2 0 2
1 3
4 0 1
1 2 3 4
2 1000000000 3000000000
1000000000 1000000000
```




```output1
Alice
Alice
Bob
Alice
```



## Note

<p>In the first test case, Alice could get $9$ using the following operations: $7 + 2 = 9$.</p><p>In the second test case, Alice could get $2$ using this operations: $(0 + 1) \oplus 3 = 2$.</p><p>In the third test case, Bob started with $x+3 = 0+3=3$ and could get $1$ this way: $(((3 + 1) + 2) \oplus 3) \oplus 4 = 1$.</p>
