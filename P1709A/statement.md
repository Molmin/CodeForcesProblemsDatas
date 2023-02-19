## Description

<div><p>There are three doors in front of you, numbered from $1$ to $3$ from left to right. Each door has a lock on it, which can only be opened with a key with the same number on it as the number on the door.</p><p>There are three keys&nbsp;— one for each door. Two of them are hidden behind the doors, so that there is no more than one key behind each door. So two doors have one key behind them, one door doesn't have a key behind it. To obtain a key hidden behind a door, you should first unlock that door. The remaining key is in your hands.</p><p>Can you open all the doors?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 18$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $x$ ($1 \le x \le 3$)&nbsp;— the number on the key in your hands.</p><p>The second line contains three integers $a, b$ and $c$ ($0 \le a, b, c \le 3$)&nbsp;— the number on the key behind each of the doors. If there is no key behind the door, the number is equal to $0$.</p><p>Values $1, 2$ and $3$ appear exactly once among $x, a, b$ and $c$.</p></div><div class="output-specification"><p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if you can open all the doors. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 18$)&nbsp;— the number of testcases.</p><p>The first line of each testcase contains a single integer $x$ ($1 \le x \le 3$)&nbsp;— the number on the key in your hands.</p><p>The second line contains three integers $a, b$ and $c$ ($0 \le a, b, c \le 3$)&nbsp;— the number on the key behind each of the doors. If there is no key behind the door, the number is equal to $0$.</p><p>Values $1, 2$ and $3$ appear exactly once among $x, a, b$ and $c$.</p>

## Output

<p>For each testcase, print "<span class="tex-font-style-tt">YES</span>" if you can open all the doors. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1|2,3,6,7
4
3
0 1 2
1
0 3 2
2
3 1 0
2
1 3 0
```




```output1
YES
NO
YES
NO
```


