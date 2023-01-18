## Description

<div><p>The coronation of King Berl XXII is soon! The whole royal family, including $n$ daughters of Berl XXII, will be present.</p><p>The King has ordered his jeweler to assemble $n$ beautiful necklaces, so each of the princesses could wear exactly one necklace during the ceremony — and now these necklaces are finished. Each necklace consists of $m$ gems attached to a gold chain. There are two types of gems used in the necklaces — emeralds and sapphires. So, each necklace can be represented by a sequence of $m$ gems (listed from left to right), and each gem is either an emerald or a sapphire. Formally, the $i$-th necklace can be represented by a binary string $s_i$ of length $m$; if the $j$-th character of $s_i$ is <span class="tex-font-style-tt">0</span>, then the $j$-th gem in the $i$-th necklace is an emerald; otherwise, this gem is a sapphire.</p><p>Now, looking at the necklaces, the King is afraid that some of his daughters may envy the other daughters' necklaces. He wants all necklaces to look <span class="tex-font-style-it">similar</span>. Two necklaces are considered <span class="tex-font-style-it">similar</span> if there are at least $k$ positions where these necklaces contain the same type of gems.</p><p>For example, if there is a necklace represented by a sequence <span class="tex-font-style-tt">01010111</span> and a necklace represented by a sequence <span class="tex-font-style-tt">01100000</span>, then there are $3$ positions where these necklaces contain the same type of gems (both first gems are emeralds, both second gems are sapphires, and both fifth gems are emeralds). So if $k = 3$, these necklaces are <span class="tex-font-style-it">similar</span>, and if $k = 4$, they are not <span class="tex-font-style-it">similar</span>.</p><p>The King thinks that if two of his daughters notice that their necklaces are not <span class="tex-font-style-it">similar</span>, then they may have a conflict — and, obviously, he doesn't want any conflicts during the coronation! So Berl XXII wants to tell some of his daughters to wear their necklaces backward. If a necklace is worn backward, then the sequence of gems in this necklace is reversed. For example, if a necklace is represented by a sequence <span class="tex-font-style-tt">01100</span>, then, if worn backward, it would be represented by a sequence <span class="tex-font-style-tt">00110</span>. The King wants to find the minimum number of necklaces to be worn backward during the coronation so that there are no conflicts.</p><p>Berl XXII is too busy with preparation for the coronation, so he ordered you to resolve this issue for him. Help him — and he will give you a truly royal reward! </p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 50$) — the number of test cases. Then the test cases follow.</p><p>Each test case begins with a line containing three integers $n$, $m$ and $k$ ($2 \le n \le 50$, $1 \le k \le m \le 50$) — the number of necklaces, the number of gems in each necklace, and the minimum number of positions where two necklaces have to have the same type of gems in order to look similar, respectively.</p><p>Then $n$ lines follow, the $i$-th of them contains a binary string $s_i$ of length $m$ representing the $i$-th necklace.</p></div><div class="output-specification"><p>For each test case, print the answer as follows.</p><p>If it is impossible to avoid the conflict, print <span class="tex-font-style-tt">-1</span> on a single line. In this case you should not output anything else for that test case.</p><p>Otherwise, the first line of the test case answer should contain the single integer $d$ — the minimum number of necklaces that are to be worn backward. The second line of the test case answer should contain the numbers of these necklaces (integers from $1$ to $n$) in any order. If $d = 0$ then leave the second line of the test case answer empty. If there are multiple answers, you may print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 50$) — the number of test cases. Then the test cases follow.</p><p>Each test case begins with a line containing three integers $n$, $m$ and $k$ ($2 \le n \le 50$, $1 \le k \le m \le 50$) — the number of necklaces, the number of gems in each necklace, and the minimum number of positions where two necklaces have to have the same type of gems in order to look similar, respectively.</p><p>Then $n$ lines follow, the $i$-th of them contains a binary string $s_i$ of length $m$ representing the $i$-th necklace.</p>

## Output

<p>For each test case, print the answer as follows.</p><p>If it is impossible to avoid the conflict, print <span class="tex-font-style-tt">-1</span> on a single line. In this case you should not output anything else for that test case.</p><p>Otherwise, the first line of the test case answer should contain the single integer $d$ — the minimum number of necklaces that are to be worn backward. The second line of the test case answer should contain the numbers of these necklaces (integers from $1$ to $n$) in any order. If $d = 0$ then leave the second line of the test case answer empty. If there are multiple answers, you may print any of them.</p>





```input1
5
5 7 2
1010100
0010101
1111010
1000010
0000101
6 9 3
011111110
100111000
111100000
000111111
110100111
111110111
3 4 2
0001
1000
0000
3 4 4
0001
1000
0000
2 4 3
0001
1000
```




```output1
2
1 3 
1
3 
0

-1
1
1
```


