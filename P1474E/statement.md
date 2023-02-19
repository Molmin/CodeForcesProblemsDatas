## Description

<div><p>Lunar rover finally reached planet <span class="tex-font-style-tt">X</span>. After landing, he met an obstacle, that contains permutation $p$ of length $n$. Scientists found out, that to overcome an obstacle, the robot should make $p$ an identity permutation (make $p_i = i$ for all $i$).</p><p>Unfortunately, scientists can't control the robot. Thus the only way to make $p$ an identity permutation is applying the following operation to $p$ multiple times: </p><ul> <li> Select two indices $i$ and $j$ ($i \neq j$), such that $p_j = i$ and swap the values of $p_i$ and $p_j$. It takes robot $(j - i)^2$ seconds to do this operation. </li></ul> Positions $i$ and $j$ are selected by the robot (scientists can't control it). He will apply this operation while $p$ isn't an identity permutation. We can show that the robot will make no more than $n$ operations regardless of the choice of $i$ and $j$ on each operation.<p>Scientists asked you to find out the maximum possible time it will take the robot to finish making $p$ an identity permutation (i.&nbsp;e. worst-case scenario), so they can decide whether they should construct a new lunar rover or just rest and wait. They won't believe you without proof, so you should build an example of $p$ and robot's operations that maximizes the answer.</p><p>For a better understanding of the statement, read the sample description.</p></div><div class="input-specification"><p>The first line of input contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each of next $t$ lines contains the single integer $n$ ($2 \leq n \leq 10^5$)&nbsp;– the length of $p$.</p><p>Note, that $p$ is not given to you. You should find the maximum possible time over all permutations of length $n$.</p><p>It is guaranteed, that the total sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case in the first line, print how many seconds will the robot spend in the worst case.</p><p>In the next line, print the initial value of $p$ that you used to construct an answer.</p><p>In the next line, print the number of operations $m \leq n$ that the robot makes in your example.</p><p>In the each of next $m$ lines print two integers $i$ and $j$&nbsp;— indices of positions that the robot will swap on this operation. Note that $p_j = i$ must holds (at the time of operation).</p></div>

## Input

<p>The first line of input contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each of next $t$ lines contains the single integer $n$ ($2 \leq n \leq 10^5$)&nbsp;– the length of $p$.</p><p>Note, that $p$ is not given to you. You should find the maximum possible time over all permutations of length $n$.</p><p>It is guaranteed, that the total sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case in the first line, print how many seconds will the robot spend in the worst case.</p><p>In the next line, print the initial value of $p$ that you used to construct an answer.</p><p>In the next line, print the number of operations $m \leq n$ that the robot makes in your example.</p><p>In the each of next $m$ lines print two integers $i$ and $j$&nbsp;— indices of positions that the robot will swap on this operation. Note that $p_j = i$ must holds (at the time of operation).</p>





```input1
3
2
3
3
```




```output1
1
2 1
1
2 1
5
2 3 1
2
1 3
3 2
5
2 3 1
2
1 3
2 3
```



## Note

<p>For $n = 2$, $p$ can be either $[1, 2]$ or $[2, 1]$. In the first case $p$ is already identity, otherwise robot will make it an identity permutation in $1$ second regardless of choise $i$ and $j$ on the first operation.</p><p>For $n = 3$, $p$ can be equals $[2, 3, 1]$.</p><ul> <li> If robot will select $i = 3, j = 2$ on the first operation, $p$ will become $[2, 1, 3]$ in one second. Now robot can select only $i = 1, j = 2$ or $i = 2, j = 1$. In both cases, $p$ will become identity in one more second ($2$ seconds in total).</li><li> If robot will select $i = 1, j = 3$ on the first operation, $p$ will become $[1, 3, 2]$ in four seconds. Regardless of choise of $i$ and $j$ on the second operation, $p$ will become identity in five seconds. </li></ul><p>We can show, that for permutation of length $3$ robot will always finish all operation in no more than $5$ seconds.</p>
