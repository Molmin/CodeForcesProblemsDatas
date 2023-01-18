## Description

<div><p>The new camp by widely-known over the country Spring Programming Camp is going to start soon. Hence, all the team of friendly curators and teachers started composing the camp's schedule. After some continuous discussion, they came up with a schedule $s$, which can be represented as a binary string, in which the $i$-th symbol is '<span class="tex-font-style-tt">1</span>' if students will write the contest in the $i$-th day and '<span class="tex-font-style-tt">0</span>' if they will have a day off.</p><p>At the last moment Gleb said that the camp will be the most productive if it runs with the schedule $t$ (which can be described in the same format as schedule $s$). Since the number of days in the current may be different from number of days in schedule $t$, Gleb required that the camp's schedule must be altered so that the number of occurrences of $t$ in it as a substring is maximum possible. At the same time, <span class="tex-font-style-bf">the number of contest days and days off shouldn't change</span>, only their order may change.</p><p>Could you rearrange the schedule in the best possible way?</p></div><div class="input-specification"><p>The first line contains string $s$ ($1 \leqslant |s| \leqslant 500\,000$), denoting the current project of the camp's schedule.</p><p>The second line contains string $t$ ($1 \leqslant |t| \leqslant 500\,000$), denoting the optimal schedule according to Gleb.</p><p>Strings $s$ and $t$ contain characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only.</p></div><div class="output-specification"><p>In the only line print the schedule having the largest number of substrings equal to $t$. Printed schedule should consist of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only and the number of zeros should be equal to the number of zeros in $s$ and the number of ones should be equal to the number of ones in $s$.</p><p>In case there multiple optimal schedules, print any of them.</p></div>

## Input

<p>The first line contains string $s$ ($1 \leqslant |s| \leqslant 500\,000$), denoting the current project of the camp's schedule.</p><p>The second line contains string $t$ ($1 \leqslant |t| \leqslant 500\,000$), denoting the optimal schedule according to Gleb.</p><p>Strings $s$ and $t$ contain characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only.</p>

## Output

<p>In the only line print the schedule having the largest number of substrings equal to $t$. Printed schedule should consist of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' only and the number of zeros should be equal to the number of zeros in $s$ and the number of ones should be equal to the number of ones in $s$.</p><p>In case there multiple optimal schedules, print any of them.</p>





```input1
101101
110
```




```input2
10010110
100011
```




```input3
10
11100
```




```output1
110110
```




```output2
01100011
```




```output3
01
```



## Note

<p>In the first example there are two occurrences, one starting from first position and one starting from fourth position.</p><p>In the second example there is only one occurrence, which starts from third position. Note, that the answer is not unique. For example, if we move the first day (which is a day off) to the last position, the number of occurrences of $t$ wouldn't change.</p><p>In the third example it's impossible to make even a single occurrence.</p>
