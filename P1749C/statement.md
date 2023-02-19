## Description

<div><p>Alice and Bob are playing a game. They have an array of positive integers $a$ of size $n$.</p><p>Before starting the game, Alice chooses an integer $k \ge 0$. The game lasts for $k$ stages, the stages are numbered from $1$ to $k$. During the $i$-th stage, Alice must remove an element from the array that is less than or equal to $k - i + 1$. After that, if the array is not empty, Bob must add $k - i + 1$ to an arbitrary element of the array. Note that both Alice's move and Bob's move are two parts of the same stage of the game. If Alice can't delete an element during some stage, she loses. If the $k$-th stage ends and Alice hasn't lost yet, she wins.</p><p>Your task is to determine the maximum value of $k$ such that Alice can win if both players play optimally. Bob plays against Alice, so he tries to make her lose the game, if it's possible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the size of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the maximum value of $k$ such that Alice can win if both players play optimally.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 100$)&nbsp;— the size of the array $a$.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p>

## Output

<p>For each test case, print one integer&nbsp;— the maximum value of $k$ such that Alice can win if both players play optimally.</p>





```input1|2,3,6,7
4
3
1 1 2
4
4 4 4 4
1
1
5
1 3 2 1 1
```




```output1
2
0
1
3
```


