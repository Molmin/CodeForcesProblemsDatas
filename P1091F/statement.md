## Description

<div><p>Bob is a duck. He wants to get to Alice's nest, so that those two can duck!</p><center> <img class="tex-graphics" src="file://Qy7IBFc2.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-it">Duck is the ultimate animal! (Image courtesy of See Bang)</span> </center><p>The journey can be represented as a straight line, consisting of $n$ segments. Bob is located to the left of the first segment, while Alice's nest is on the right of the last segment. Each segment has a length in meters, and also terrain type: grass, water or lava. </p><p>Bob has three movement types: swimming, walking and flying. He can switch between them or change his direction at any point in time (even when he is located at a non-integer coordinate), and doing so doesn't require any extra time. Bob can swim only on the water, walk only on the grass and fly over <span class="tex-font-style-bf">any</span> terrain. Flying one meter takes $1$ second, swimming one meter takes $3$ seconds, and finally walking one meter takes $5$ seconds.</p><p>Bob has a finite amount of energy, called stamina. Swimming and walking is relaxing for him, so he gains $1$ stamina for every meter he walks or swims. On the other hand, flying is quite tiring, and he spends $1$ stamina for every meter flown. Staying in place does not influence his stamina at all. Of course, his stamina can never become negative. Initially, his stamina is zero.</p><p>What is the shortest possible time in which he can reach Alice's nest? </p></div><div class="input-specification"><p>The first line contains a single integer $n$&nbsp;($1 \leq n \leq 10^5$)&nbsp;— the number of segments of terrain. </p><p>The second line contains $n$ integers $l_1, l_2, \dots, l_n$&nbsp;($1 \leq l_i \leq 10^{12}$). The $l_i$ represents the length of the $i$-th terrain segment in meters.</p><p>The third line contains a string $s$ consisting of $n$ characters "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">W</span>", "<span class="tex-font-style-tt">L</span>", representing <span class="tex-font-style-bf">G</span>rass, <span class="tex-font-style-bf">W</span>ater and <span class="tex-font-style-bf">L</span>ava, respectively. </p><p>It is guaranteed that the first segment is not Lava.</p></div><div class="output-specification"><p>Output a single integer $t$&nbsp;— the minimum time Bob needs to reach Alice. </p></div>

## Input

<p>The first line contains a single integer $n$&nbsp;($1 \leq n \leq 10^5$)&nbsp;— the number of segments of terrain. </p><p>The second line contains $n$ integers $l_1, l_2, \dots, l_n$&nbsp;($1 \leq l_i \leq 10^{12}$). The $l_i$ represents the length of the $i$-th terrain segment in meters.</p><p>The third line contains a string $s$ consisting of $n$ characters "<span class="tex-font-style-tt">G</span>", "<span class="tex-font-style-tt">W</span>", "<span class="tex-font-style-tt">L</span>", representing <span class="tex-font-style-bf">G</span>rass, <span class="tex-font-style-bf">W</span>ater and <span class="tex-font-style-bf">L</span>ava, respectively. </p><p>It is guaranteed that the first segment is not Lava.</p>

## Output

<p>Output a single integer $t$&nbsp;— the minimum time Bob needs to reach Alice. </p>





```input1
1
10
G
```




```input2
2
10 10
WL
```




```input3
2
1 2
WL
```




```input4
3
10 10 10
GLW
```




```output1
30
```




```output2
40
```




```output3
8
```




```output4
80
```



## Note

<p>In the first sample, Bob first walks $5$ meters in $25$ seconds. Then he flies the remaining $5$ meters in $5$ seconds.</p><p>In the second sample, Bob first swims $10$ meters in $30$ seconds. Then he flies over the patch of lava for $10$ seconds.</p><p>In the third sample, the water pond is much smaller. Bob first swims over the water pond, taking him $3$ seconds. However, he cannot fly over the lava just yet, as he only has one stamina while he needs two. So he swims back for half a meter, and then half a meter forward, taking him $3$ seconds in total. Now he has $2$ stamina, so he can spend $2$ seconds flying over the lava.</p><p>In the fourth sample, he walks for $50$ seconds, flies for $10$ seconds, swims for $15$ seconds, and finally flies for $5$ seconds.</p>
