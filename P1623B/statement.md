## Description

<div><p>Alice and Bob play the following game. Alice has a set $S$ of disjoint ranges of integers, initially containing only one range $[1, n]$. In one turn, Alice picks a range $[l, r]$ from the set $S$ and asks Bob to pick a number in the range. Bob chooses a number $d$ ($l \le d \le r$). Then Alice removes $[l, r]$ from $S$ and puts into the set $S$ the range $[l, d - 1]$ (if $l \le d - 1$) and the range $[d + 1, r]$ (if $d + 1 \le r$). The game ends when the set $S$ is empty. We can show that the number of turns in each game is exactly $n$.</p><p>After playing the game, Alice remembers all the ranges $[l, r]$ she picked from the set $S$, but Bob does not remember any of the numbers that he picked. But Bob is smart, and he knows he can find out his numbers $d$ from Alice's ranges, and so he asks you for help with your programming skill.</p><p>Given the list of ranges that Alice has picked ($[l, r]$), for each range, help Bob find the number $d$ that Bob has picked.</p><p>We can show that there is always a unique way for Bob to choose his number for a list of valid ranges picked by Alice.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 1000$).</p><p>Each of the next $n$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le n$), denoting the range $[l, r]$ that Alice picked at some point.</p><p>Note that the ranges are given <span class="tex-font-style-bf">in no particular order</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$, and the ranges for each test case are from a valid game.</p></div><div class="output-specification"><p>For each test case print $n$ lines. Each line should contain three integers $l$, $r$, and $d$, denoting that for Alice's range $[l, r]$ Bob picked the number $d$.</p><p>You can print the lines in <span class="tex-font-style-bf">any order</span>. We can show that the answer is unique.</p><p>It is not required to print a new line after each test case. The new lines in the output of the example are for readability only. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 1000$).</p><p>Each of the next $n$ lines contains two integers $l$ and $r$ ($1 \le l \le r \le n$), denoting the range $[l, r]$ that Alice picked at some point.</p><p>Note that the ranges are given <span class="tex-font-style-bf">in no particular order</span>.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $1000$, and the ranges for each test case are from a valid game.</p>

## Output

<p>For each test case print $n$ lines. Each line should contain three integers $l$, $r$, and $d$, denoting that for Alice's range $[l, r]$ Bob picked the number $d$.</p><p>You can print the lines in <span class="tex-font-style-bf">any order</span>. We can show that the answer is unique.</p><p>It is not required to print a new line after each test case. The new lines in the output of the example are for readability only. </p>





```input1
4
1
1 1
3
1 3
2 3
2 2
6
1 1
3 5
4 4
3 6
4 5
1 6
5
1 5
1 2
4 5
2 2
4 4
```




```output1
1 1 1

1 3 1
2 2 2
2 3 3

1 1 1
3 5 3
4 4 4
3 6 6
4 5 5
1 6 2

1 5 3
1 2 1
4 5 5
2 2 2
4 4 4
```



## Note

<p>In the first test case, there is only 1 range $[1, 1]$. There was only one range $[1, 1]$ for Alice to pick, and there was only one number $1$ for Bob to pick.</p><p>In the second test case, $n = 3$. Initially, the set contains only one range $[1, 3]$. </p><ul> <li> Alice picked the range $[1, 3]$. Bob picked the number $1$. Then Alice put the range $[2, 3]$ back to the set, which after this turn is the only range in the set. </li><li> Alice picked the range $[2, 3]$. Bob picked the number $3$. Then Alice put the range $[2, 2]$ back to the set. </li><li> Alice picked the range $[2, 2]$. Bob picked the number $2$. The game ended. </li></ul><p>In the fourth test case, the game was played with $n = 5$. Initially, the set contains only one range $[1, 5]$. The game's turn is described in the following table. </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Game turn</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Alice's picked range</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Bob's picked number</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">The range set after</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">Before the game start</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \{ [1, 5] \} $</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">1</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$[1, 5]$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \{ [1, 2], [4, 5] \}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">2</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$[1, 2]$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \{ [2, 2], [4, 5] \} $</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">3</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$[4, 5]$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \{ [2, 2], [4, 4] \} $</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">4</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$[2, 2]$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \{ [4, 4] \} $</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">5</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$[4, 4]$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$ \{ \} $ (empty set)</td></tr></tbody></table> </center>
