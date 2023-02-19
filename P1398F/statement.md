## Description

<div><p>Alice and Bob play a game. The game consists of several sets, and each set consists of several rounds. Each round is won either by Alice or by Bob, and the set ends when one of the players has won $x$ rounds in a row. For example, if Bob won five rounds in a row and $x = 2$, then two sets ends.</p><p>You know that Alice and Bob have already played $n$ rounds, and you know the results of some rounds. For each $x$ from $1$ to $n$, calculate the maximum possible number of sets that could have already finished if each set lasts until one of the players wins $x$ rounds in a row. It is possible that the last set is still not finished — in that case, you should not count it in the answer.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 10^6$)&nbsp;— the number of rounds.</p><p>The second line contains one string $s$ of length $n$ — the descriptions of rounds. If the $i$-th element of the string is <span class="tex-font-style-tt">0</span>, then Alice won the $i$-th round; if it is <span class="tex-font-style-tt">1</span>, then Bob won the $i$-th round, and if it is <span class="tex-font-style-tt">?</span>, then you don't know who won the $i$-th round.</p></div><div class="output-specification"><p>In the only line print $n$ integers. The $i$-th integer should be equal to the maximum possible number of sets that could have already finished if each set lasts until one of the players wins $i$ rounds in a row.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 10^6$)&nbsp;— the number of rounds.</p><p>The second line contains one string $s$ of length $n$ — the descriptions of rounds. If the $i$-th element of the string is <span class="tex-font-style-tt">0</span>, then Alice won the $i$-th round; if it is <span class="tex-font-style-tt">1</span>, then Bob won the $i$-th round, and if it is <span class="tex-font-style-tt">?</span>, then you don't know who won the $i$-th round.</p>

## Output

<p>In the only line print $n$ integers. The $i$-th integer should be equal to the maximum possible number of sets that could have already finished if each set lasts until one of the players wins $i$ rounds in a row.</p>





```input1
6
11?000
```




```input2
5
01?01
```




```input3
12
???1??????1?
```




```output1
6 3 2 1 0 0
```




```output2
5 1 0 0 0
```




```output3
12 6 4 3 2 2 1 1 1 1 1 1
```



## Note

<p>Let's consider the first test case:</p><ul> <li> if $x = 1$ and $s = 110000$ or $s = 111000$ then there are six finished sets; </li><li> if $x = 2$ and $s = 110000$ then there are three finished sets; </li><li> if $x = 3$ and $s = 111000$ then there are two finished sets; </li><li> if $x = 4$ and $s = 110000$ then there is one finished set; </li><li> if $x = 5$ then there are no finished sets; </li><li> if $x = 6$ then there are no finished sets. </li></ul>
