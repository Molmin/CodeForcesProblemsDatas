## Description

<div><p>Recently you have bought a snow walking robot and brought it home. Suppose your home is a cell $(0, 0)$ on an infinite grid.</p><p>You also have the sequence of instructions of this robot. It is written as the string $s$ consisting of characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">D</span>'. If the robot is in the cell $(x, y)$ right now, he can move to one of the adjacent cells (depending on the current instruction).</p><ul> <li> If the current instruction is '<span class="tex-font-style-tt">L</span>', then the robot can move to the left to $(x - 1, y)$; </li><li> if the current instruction is '<span class="tex-font-style-tt">R</span>', then the robot can move to the right to $(x + 1, y)$; </li><li> if the current instruction is '<span class="tex-font-style-tt">U</span>', then the robot can move to the top to $(x, y + 1)$; </li><li> if the current instruction is '<span class="tex-font-style-tt">D</span>', then the robot can move to the bottom to $(x, y - 1)$. </li></ul><p>You've noticed the warning on the last page of the manual: if the robot visits some cell (<span class="tex-font-style-bf">except</span> $(0, 0)$) twice then it breaks.</p><p>So the sequence of instructions is valid if the robot starts in the cell $(0, 0)$, performs the given instructions, visits no cell other than $(0, 0)$ two or more times and ends the path in the cell $(0, 0)$. Also cell $(0, 0)$ should be visited <span class="tex-font-style-bf">at most</span> two times: at the beginning and at the end (if the path is empty then it is visited only once). For example, the following sequences of instructions are considered valid: "<span class="tex-font-style-tt">UD</span>", "<span class="tex-font-style-tt">RL</span>", "<span class="tex-font-style-tt">UUURULLDDDDLDDRRUU</span>", and the following are considered invalid: "<span class="tex-font-style-tt">U</span>" (the endpoint is not $(0, 0)$) and "<span class="tex-font-style-tt">UUDD</span>" (the cell $(0, 1)$ is visited twice).</p><p>The initial sequence of instructions, however, might be not valid. You don't want your robot to break so you decided to reprogram it in the following way: you will remove some (possibly, all or none) instructions from the initial sequence of instructions, then rearrange the remaining instructions as you wish and turn on your robot to move. </p><p>Your task is to remove as few instructions from the initial sequence as possible and rearrange the remaining ones so that the sequence is valid. Report the valid sequence of the maximum length you can obtain.</p><p>Note that you can choose <span class="tex-font-style-bf">any</span> order of remaining instructions (you don't need to minimize the number of swaps or any other similar metric).</p><p>You have to answer $q$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^4$) — the number of test cases.</p><p>The next $q$ lines contain test cases. The $i$-th test case is given as the string $s$ consisting of at least $1$ and no more than $10^5$ characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">D</span>' — the initial sequence of instructions.</p><p>It is guaranteed that the sum of $|s|$ (where $|s|$ is the length of $s$) does not exceed $10^5$ over all test cases ($\sum |s| \le 10^5$).</p></div><div class="output-specification"><p>For each test case print the answer on it. In the first line print the maximum number of remaining instructions. In the second line print the valid sequence of remaining instructions $t$ the robot has to perform. The moves are performed from left to right in the order of the printed sequence. If there are several answers, you can print any. If the answer is $0$, you are allowed to print an empty line (but you can don't print it).</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 2 \cdot 10^4$) — the number of test cases.</p><p>The next $q$ lines contain test cases. The $i$-th test case is given as the string $s$ consisting of at least $1$ and no more than $10^5$ characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">U</span>' and '<span class="tex-font-style-tt">D</span>' — the initial sequence of instructions.</p><p>It is guaranteed that the sum of $|s|$ (where $|s|$ is the length of $s$) does not exceed $10^5$ over all test cases ($\sum |s| \le 10^5$).</p>

## Output

<p>For each test case print the answer on it. In the first line print the maximum number of remaining instructions. In the second line print the valid sequence of remaining instructions $t$ the robot has to perform. The moves are performed from left to right in the order of the printed sequence. If there are several answers, you can print any. If the answer is $0$, you are allowed to print an empty line (but you can don't print it).</p>





```input1
6
LRU
DURLDRUDRULRDURDDL
LRUDDLRUDRUL
LLLLRRRR
URDUR
LLL
```




```output1
2
LR
14
RUURDDDDLLLUUR
12
ULDDDRRRUULL
2
LR
2
UD
0
```



## Note

<p>There are only two possible answers in the first test case: "<span class="tex-font-style-tt">LR</span>" and "<span class="tex-font-style-tt">RL</span>".</p><p>The picture corresponding to the second test case:</p><center> <img class="tex-graphics" src="file://j9Je7YAb.png" style="max-width: 100.0%;max-height: 100.0%;"> Note that the direction of traverse does not matter </center><p>Another correct answer to the third test case: "<span class="tex-font-style-tt">URDDLLLUURDR</span>".</p>
