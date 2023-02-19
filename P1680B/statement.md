## Description

<div><p>There is a field divided into $n$ rows and $m$ columns. Some cells are empty (denoted as <span class="tex-font-style-tt">E</span>), other cells contain robots (denoted as <span class="tex-font-style-tt">R</span>).</p><p>You can send a command to <span class="tex-font-style-bf">all robots</span> at the same time. The command can be of one of the four types:</p><ul> <li> move up; </li><li> move right; </li><li> move down; </li><li> move left. </li></ul><p>When you send a command, <span class="tex-font-style-bf">all robots at the same time</span> attempt to take one step in the direction you picked. If a robot tries to move outside the field, it explodes; otherwise, <span class="tex-font-style-bf">every robot</span> moves to an adjacent cell in the chosen direction.</p><p>You can send as many commands as you want (possibly, zero), in any order. Your goal is to make at least one robot reach the upper left corner of the field. Can you do this without forcing any of the robots to explode?</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>Each test case starts with a line containing two integers $n$ and $m$ ($1 \le n, m \le 5$)&nbsp;— the number of rows and the number of columns, respectively. Then $n$ lines follow; each of them contains a string of $m$ characters. Each character is either <span class="tex-font-style-tt">E</span> (empty cell} or <span class="tex-font-style-tt">R</span> (robot).</p><p>Additional constraint on the input: in each test case, there is at least one robot on the field.</p></div><div class="output-specification"><p>If it is possible to make at least one robot reach the upper left corner of the field so that no robot explodes, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5000$)&nbsp;— the number of test cases.</p><p>Each test case starts with a line containing two integers $n$ and $m$ ($1 \le n, m \le 5$)&nbsp;— the number of rows and the number of columns, respectively. Then $n$ lines follow; each of them contains a string of $m$ characters. Each character is either <span class="tex-font-style-tt">E</span> (empty cell} or <span class="tex-font-style-tt">R</span> (robot).</p><p>Additional constraint on the input: in each test case, there is at least one robot on the field.</p>

## Output

<p>If it is possible to make at least one robot reach the upper left corner of the field so that no robot explodes, print <span class="tex-font-style-tt">YES</span>. Otherwise, print <span class="tex-font-style-tt">NO</span>.</p>





```input1
6
1 3
ERR
2 2
ER
RE
2 2
ER
ER
1 1
R
4 3
EEE
EEE
ERR
EER
3 3
EEE
EER
REE
```




```output1
YES
NO
YES
YES
YES
NO
```



## Note

<p>Explanations for test cases of the example:</p><ol> <li> in the first test case, it is enough to send a command to move left. </li><li> in the second test case, if you try to send any command, at least one robot explodes. </li><li> in the third test case, it is enough to send a command to move left. </li><li> in the fourth test case, there is already a robot in the upper left corner. </li><li> in the fifth test case, the sequence "move up, move left, move up" leads one robot to the upper left corner; </li><li> in the sixth test case, if you try to move any robot to the upper left corner, at least one other robot explodes. </li></ol>
