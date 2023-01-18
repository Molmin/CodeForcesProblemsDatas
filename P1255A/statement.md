## Description

<div><p>Bob watches TV every day. He always sets the volume of his TV to $b$. However, today he is angry to find out someone has changed the volume to $a$. Of course, Bob has a remote control that can change the volume.</p><p>There are six buttons ($-5, -2, -1, +1, +2, +5$) on the control, which in one press can either increase or decrease the current volume by $1$, $2$, or $5$. The volume can be arbitrarily large, but can never be negative. In other words, Bob cannot press the button if it causes the volume to be lower than $0$.</p><p>As Bob is so angry, he wants to change the volume to $b$ using as few button presses as possible. However, he forgets how to do such simple calculations, so he asks you for help. Write a program that given $a$ and $b$, finds the minimum number of presses to change the TV volume from $a$ to $b$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $T$ ($1 \le T \le 1\,000$). Then the descriptions of the test cases follow.</p><p>Each test case consists of one line containing two integers $a$ and $b$ ($0 \le a, b \le 10^{9}$)&nbsp;— the current volume and Bob's desired volume, respectively.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum number of presses to change the TV volume from $a$ to $b$. If Bob does not need to change the volume (i.e. $a=b$), then print $0$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $T$ ($1 \le T \le 1\,000$). Then the descriptions of the test cases follow.</p><p>Each test case consists of one line containing two integers $a$ and $b$ ($0 \le a, b \le 10^{9}$)&nbsp;— the current volume and Bob's desired volume, respectively.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum number of presses to change the TV volume from $a$ to $b$. If Bob does not need to change the volume (i.e. $a=b$), then print $0$.</p>





```input1
3
4 0
5 14
3 9
```




```output1
2
3
2
```



## Note

<p>In the first example, Bob can press the $-2$ button twice to reach $0$. Note that Bob can not press $-5$ when the volume is $4$ since it will make the volume negative. </p><p>In the second example, one of the optimal ways for Bob is to press the $+5$ twice, then press $-1$ once.</p><p>In the last example, Bob can press the $+5$ once, then press $+1$. </p>
