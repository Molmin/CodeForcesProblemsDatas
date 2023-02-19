## Description

<div><p>Alice and Bob have decided to play the game "Rock, Paper, Scissors". </p><p>The game consists of several rounds, each round is independent of each other. In each round, both players show one of the following things at the same time: rock, paper or scissors. If both players showed the same things then the round outcome is a draw. Otherwise, the following rules applied:</p><ul> <li> if one player showed rock and the other one showed scissors, then the player who showed rock is considered the winner and the other one is considered the loser; </li><li> if one player showed scissors and the other one showed paper, then the player who showed scissors is considered the winner and the other one is considered the loser; </li><li> if one player showed paper and the other one showed rock, then the player who showed paper is considered the winner and the other one is considered the loser. </li></ul><p>Alice and Bob decided to play exactly $n$ rounds of the game described above. Alice decided to show rock $a_1$ times, show scissors $a_2$ times and show paper $a_3$ times. Bob decided to show rock $b_1$ times, show scissors $b_2$ times and show paper $b_3$ times. Though, both Alice and Bob <span class="tex-font-style-bf">did not choose</span> the sequence in which they show things. It is guaranteed that $a_1 + a_2 + a_3 = n$ and $b_1 + b_2 + b_3 = n$.</p><p>Your task is to find two numbers:</p><ol> <li> the minimum number of round Alice can win; </li><li> the maximum number of rounds Alice can win. </li></ol></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 10^{9}$) — the number of rounds.</p><p>The second line of the input contains three integers $a_1, a_2, a_3$ ($0 \le a_i \le n$) — the number of times Alice will show rock, scissors and paper, respectively. It is guaranteed that $a_1 + a_2 + a_3 = n$.</p><p>The third line of the input contains three integers $b_1, b_2, b_3$ ($0 \le b_j \le n$) — the number of times Bob will show rock, scissors and paper, respectively. It is guaranteed that $b_1 + b_2 + b_3 = n$.</p></div><div class="output-specification"><p>Print two integers: the minimum and the maximum number of rounds Alice can win.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 10^{9}$) — the number of rounds.</p><p>The second line of the input contains three integers $a_1, a_2, a_3$ ($0 \le a_i \le n$) — the number of times Alice will show rock, scissors and paper, respectively. It is guaranteed that $a_1 + a_2 + a_3 = n$.</p><p>The third line of the input contains three integers $b_1, b_2, b_3$ ($0 \le b_j \le n$) — the number of times Bob will show rock, scissors and paper, respectively. It is guaranteed that $b_1 + b_2 + b_3 = n$.</p>

## Output

<p>Print two integers: the minimum and the maximum number of rounds Alice can win.</p>





```input1
2
0 1 1
1 1 0
```




```input2
15
5 5 5
5 5 5
```




```input3
3
0 0 3
3 0 0
```




```input4
686
479 178 29
11 145 530
```




```input5
319
10 53 256
182 103 34
```




```output1
0 1
```




```output2
0 15
```




```output3
3 3
```




```output4
22 334
```




```output5
119 226
```



## Note

<p>In the first example, Alice will not win any rounds if she shows scissors and then paper and Bob shows rock and then scissors. In the best outcome, Alice will win one round if she shows paper and then scissors, and Bob shows rock and then scissors.</p><p>In the second example, Alice will not win any rounds if Bob shows the same things as Alice each round.</p><p>In the third example, Alice always shows paper and Bob always shows rock so Alice will win all three rounds anyway.</p>
