## Description

<div><p>You are standing in front of the room with great treasures. The only thing stopping you is the door with a push-button combination lock. This lock has $d$ buttons with digits from $0$ to $d - 1$. Whenever you press a button, it stays pushed down. You can not pop back up just one button, but there is a "RESET" button&nbsp;— pressing it pops up all other buttons. Initially, no buttons are pushed down.</p><p>The door instantly opens when some specific set of digits is pushed down. Sadly, you don't know the password for it. Having read the documentation for this specific lock, you found out that there are $n$ possible passwords for this particular lock. </p><p>Find the shortest sequence of button presses, such that all possible passwords appear at least once during its execution. Any shortest correct sequence of button presses will be accepted.</p></div><div class="input-specification"><p>The first line contains two integers $d$ and $n$ ($1 \le d \le 10$; $1 \le n \le 2^d - 1$). Next $n$ lines describe possible passwords. Each line contains a string $s_i$ of $d$ zeros and ones: for all $j$ from $1$ to $d$ the $j$-th character is <span class="tex-font-style-tt">1</span> iff the button with the digit $j - 1$ must be pushed down.</p><p>All strings $s_i$ are different, and each string contains at least one <span class="tex-font-style-tt">1</span>.</p></div><div class="output-specification"><p>On the first line, print the number $k$&nbsp;— the minimum number of button presses. On the second line, print $k$ tokens, describing the sequence. Whenever you press a button with a digit, print that digit. Whenever you press "RESET", print "<span class="tex-font-style-tt">R</span>".</p></div>

## Input

<p>The first line contains two integers $d$ and $n$ ($1 \le d \le 10$; $1 \le n \le 2^d - 1$). Next $n$ lines describe possible passwords. Each line contains a string $s_i$ of $d$ zeros and ones: for all $j$ from $1$ to $d$ the $j$-th character is <span class="tex-font-style-tt">1</span> iff the button with the digit $j - 1$ must be pushed down.</p><p>All strings $s_i$ are different, and each string contains at least one <span class="tex-font-style-tt">1</span>.</p>

## Output

<p>On the first line, print the number $k$&nbsp;— the minimum number of button presses. On the second line, print $k$ tokens, describing the sequence. Whenever you press a button with a digit, print that digit. Whenever you press "RESET", print "<span class="tex-font-style-tt">R</span>".</p>





```input1
2 2
10
11
```




```input2
3 4
001
111
101
011
```




```output1
2
0 1
```




```output2
6
2 0 R 1 2 0
```



## Note

<p>In the second example, the sequence <span class="tex-font-style-tt">1 2 R 2 0 1</span> is also possible.</p>
