## Description

<div><p>You are playing a computer game. To pass the current level, you have to kill a big horde of monsters. In this horde, there are $n$ monsters standing in the row, numbered from $1$ to $n$. The $i$-th monster has $a_i$ health and a special "Death's Blessing" spell of strength $b_i$ attached to it.</p><p>You are going to kill all of them <span class="tex-font-style-it">one by one</span>. It takes exactly $h$ seconds to kill a monster with health $h$.</p><p>When the $i$-th monster dies, it casts its spell that increases the health of its <span class="tex-font-style-it">neighbors</span> by $b_i$ (the neighbors of the $j$-th monster in the row are the monsters on places $j - 1$ and $j + 1$. The first and the last monsters have only one neighbor each).</p><p>After each monster is killed, the row shrinks, so its former neighbors become adjacent to each other (so if one of them dies, the other one is affected by its spell). For example, imagine a situation with $4$ monsters with health $a = [2, 6, 7, 3]$ and spells $b = [3, 6, 0, 5]$. One of the ways to get rid of the monsters is shown below: </p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$6$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$7$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right" rowspan="2">$\xrightarrow{6\ s}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$8$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$13$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right" rowspan="2">$\xrightarrow{13\ s}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$8$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right" rowspan="2">$\xrightarrow{8\ s}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$6$</td><td class="tex-tabular-border-left tex-tabular-text-align-center" rowspan="2">$\xrightarrow{6\ s}$</td><td class="tex-tabular-text-align-center" rowspan="2">$\{\}$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$6$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$0$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right">$5$</td><td></td></tr></tbody></table> <span class="tex-font-size-small">The first row represents the health of each monster, the second one&nbsp;— the power of the spells.</span> </center><p>As a result, we can kill all monsters in $6 + 13 + 8 + 6$ $=$ $33$ seconds. Note that it's only an example and may not be the fastest way to get rid of the monsters.</p><p>What is the minimum time required to kill all monsters in the row?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of monsters in the row.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the initial health of corresponding monsters.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i \le 10^9$), where $b_i$ is the strength of the spell for the $i$-th monster.</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the minimum possible total time to kill all monsters.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the number of monsters in the row.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the initial health of corresponding monsters.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($0 \le b_i \le 10^9$), where $b_i$ is the strength of the spell for the $i$-th monster.</p><p>It's guaranteed that the sum of $n$ doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print one integer&nbsp;— the minimum possible total time to kill all monsters.</p>





```input1|2,3,4,8,9,10
4
1
10
0
3
100 1 100
1 100 1
4
2 6 7 3
3 6 0 5
2
1000000000 1000000000
1000000000 1000000000
```




```output1
10
203
26
3000000000
```



## Note

<p>In the first test case, there is only one monster that will be killed in $10$ seconds.</p><p>In the second test case, it's optimal to kill the first monster, the last monster and then the middle one. It will take $100 + 100 + (1 + 1 + 1)$ $=$ $203$ seconds.</p><p>In the third test case, it's optimal to kill the first monster, then the third one, then the fourth one and finally the second one. It will take $2 + 7 + (3 + 0) + (3 + 6 + 5)$ $=$ $26$ seconds.</p>
