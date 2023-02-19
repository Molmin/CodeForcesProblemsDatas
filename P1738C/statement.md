## Description

<div><p>Alice and Bob are playing a game on a sequence $a_1, a_2, \dots, a_n$ of length $n$. They move in turns and <span class="tex-font-style-bf">Alice moves first</span>.</p><p>In the turn of each player, he or she should select an integer and remove it from the sequence. The game ends when there is no integer left in the sequence. </p><p>Alice wins if the sum of her selected integers is <span class="tex-font-style-bf">even</span>; otherwise, Bob wins. </p><p>Your task is to determine who will win the game, if both players play optimally.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$), indicating the length of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \leq a_i \leq 10^9$), indicating the elements of the sequence.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">Alice</span>" (without quotes) if Alice wins and "<span class="tex-font-style-tt">Bob</span>" (without quotes) otherwise.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \leq t \leq 100$) — the number of test cases. The following lines contain the description of each test case.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$), indicating the length of the sequence.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \leq a_i \leq 10^9$), indicating the elements of the sequence.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">Alice</span>" (without quotes) if Alice wins and "<span class="tex-font-style-tt">Bob</span>" (without quotes) otherwise.</p>





```input1|2,3,6,7
4
3
1 3 5
4
1 3 5 7
4
1 2 3 4
4
10 20 30 40
```




```output1
Alice
Alice
Bob
Alice
```



## Note

<p>In the first and second test cases, Alice always selects two odd numbers, so the sum of her selected numbers is always even. Therefore, Alice always wins.</p><p>In the third test case, Bob has a winning strategy that he always selects a number with the same parity as Alice selects in her last turn. Therefore, Bob always wins.</p><p>In the fourth test case, Alice always selects two even numbers, so the sum of her selected numbers is always even. Therefore, Alice always wins.</p>
