## Description

<div><p>Vasya has got a robot which is situated on an infinite Cartesian plane, initially in the cell $(0, 0)$. Robot can perform the following four kinds of operations: </p><ul> <li> <span class="tex-font-style-tt">U</span> — move from $(x, y)$ to $(x, y + 1)$; </li><li> <span class="tex-font-style-tt">D</span> — move from $(x, y)$ to $(x, y - 1)$; </li><li> <span class="tex-font-style-tt">L</span> — move from $(x, y)$ to $(x - 1, y)$; </li><li> <span class="tex-font-style-tt">R</span> — move from $(x, y)$ to $(x + 1, y)$. </li></ul><p>Vasya also has got a sequence of $n$ operations. Vasya wants to modify this sequence so after performing it the robot will end up in $(x, y)$.</p><p>Vasya wants to change the sequence so the length of changed subsegment is minimum possible. This length can be calculated as follows: $maxID - minID + 1$, where $maxID$ is the maximum index of a changed operation, and $minID$ is the minimum index of a changed operation. For example, if Vasya changes <span class="tex-font-style-tt">RRRRRRR</span> to <span class="tex-font-style-tt">RLRRLRL</span>, then the operations with indices $2$, $5$ and $7$ are changed, so the length of changed subsegment is $7 - 2 + 1 = 6$. Another example: if Vasya changes <span class="tex-font-style-tt">DDDD</span> to <span class="tex-font-style-tt">DDRD</span>, then the length of changed subsegment is $1$. </p><p><span class="tex-font-style-bf">If there are no changes, then the length of changed subsegment is $0$. Changing an operation means replacing it with some operation (possibly the same); Vasya can't insert new operations into the sequence or remove them.</span></p><p>Help Vasya! Tell him the minimum length of subsegment that he needs to change so that the robot will go from $(0, 0)$ to $(x, y)$, or tell him that it's impossible.</p></div><div class="input-specification"><p>The first line contains one integer number $n~(1 \le n \le 2 \cdot 10^5)$ — the number of operations.</p><p>The second line contains the sequence of operations — a string of $n$ characters. Each character is either <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>.</p><p>The third line contains two integers $x, y~(-10^9 \le x, y \le 10^9)$ — the coordinates of the cell where the robot should end its path.</p></div><div class="output-specification"><p>Print one integer — the minimum possible length of subsegment that can be changed so the resulting sequence of operations moves the robot from $(0, 0)$ to $(x, y)$. If this change is impossible, print $-1$.</p></div>

## Input

<p>The first line contains one integer number $n~(1 \le n \le 2 \cdot 10^5)$ — the number of operations.</p><p>The second line contains the sequence of operations — a string of $n$ characters. Each character is either <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span> or <span class="tex-font-style-tt">R</span>.</p><p>The third line contains two integers $x, y~(-10^9 \le x, y \le 10^9)$ — the coordinates of the cell where the robot should end its path.</p>

## Output

<p>Print one integer — the minimum possible length of subsegment that can be changed so the resulting sequence of operations moves the robot from $(0, 0)$ to $(x, y)$. If this change is impossible, print $-1$.</p>





```input1
5
RURUU
-2 3

```




```input2
4
RULR
1 1

```




```input3
3
UUU
100 100

```




```output1
3

```




```output2
0

```




```output3
-1

```



## Note

<p>In the first example the sequence can be changed to <span class="tex-font-style-tt"><span class="tex-font-style-bf">L</span>U<span class="tex-font-style-bf">L</span>UU</span>. So the length of the changed subsegment is $3 - 1 + 1 = 3$.</p><p>In the second example the given sequence already leads the robot to $(x, y)$, so the length of the changed subsegment is $0$.</p><p>In the third example the robot can't end his path in the cell $(x, y)$.</p>
