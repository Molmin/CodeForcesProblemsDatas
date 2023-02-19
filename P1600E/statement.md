## Description

<div><p>Alice and Bob are playing a game. They are given an array $A$ of length $N$. The array consists of integers. They are building a sequence together. In the beginning, the sequence is empty. In one turn a player can remove a number from the left or right side of the array and append it to the sequence. The rule is that the sequence they are building must be strictly increasing. The winner is the player that makes the last move. Alice is playing first. Given the starting array, under the assumption that they both play optimally, who wins the game?</p></div><div class="input-specification"><p>The first line contains one integer $N$ ($1 \leq N \leq 2*10^5$) - the length of the array $A$.</p><p>The second line contains $N$ integers $A_1$, $A_2$,...,$A_N$ ($0 \leq A_i \leq 10^9$)</p></div><div class="output-specification"><p>The first and only line of output consists of one string, the name of the winner. If Alice won, print "Alice", otherwise, print "Bob".</p></div>

## Input

<p>The first line contains one integer $N$ ($1 \leq N \leq 2*10^5$) - the length of the array $A$.</p><p>The second line contains $N$ integers $A_1$, $A_2$,...,$A_N$ ($0 \leq A_i \leq 10^9$)</p>

## Output

<p>The first and only line of output consists of one string, the name of the winner. If Alice won, print "Alice", otherwise, print "Bob".</p>





```input1
1
5
```




```input2
3
5 4 5
```




```input3
6
5 8 2 1 10 9
```




```output1
Alice
```




```output2
Alice
```




```output3
Bob
```


