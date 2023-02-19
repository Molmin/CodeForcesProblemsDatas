## Description

<div><p>Mike and Joe are playing a game with some stones. Specifically, they have $n$ piles of stones of sizes $a_1, a_2, \ldots, a_n$. These piles are arranged in a circle.</p><p>The game goes as follows. Players take turns removing some positive number of stones from a pile in clockwise order starting from pile $1$. Formally, if a player removed stones from pile $i$ on a turn, the other player removes stones from pile $((i\bmod n) + 1)$ on the next turn.</p><p>If a player cannot remove any stones on their turn (because the pile is empty), they lose. Mike goes first.</p><p>If Mike and Joe play optimally, who will win?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$) &nbsp;— the number of piles.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) &nbsp;— the size of the piles.</p></div><div class="output-specification"><p>For each test case print the winner of the game, either "Mike" or "Joe" on its own line (without quotes).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$) &nbsp;— the number of piles.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) &nbsp;— the size of the piles.</p>

## Output

<p>For each test case print the winner of the game, either "Mike" or "Joe" on its own line (without quotes).</p>





```input1|2,3
2
1
37
2
100 100
```




```output1
Mike
Joe
```



## Note

<p>In the first test case, Mike just takes all $37$ stones on his first turn.</p><p>In the second test case, Joe can just copy Mike's moves every time. Since Mike went first, he will hit $0$ on the first pile one move before Joe does so on the second pile.</p>
