## Description

<div><p>You have a password which you often type — a string $s$ of length $n$. Every character of this string is one of the first $m$ lowercase Latin letters.</p><p>Since you spend a lot of time typing it, you want to buy a new keyboard.</p><p>A keyboard is a permutation of the first $m$ Latin letters. For example, if $m = 3$, then there are six possible keyboards: <span class="tex-font-style-tt">abc</span>, <span class="tex-font-style-tt">acb</span>, <span class="tex-font-style-tt">bac</span>, <span class="tex-font-style-tt">bca</span>, <span class="tex-font-style-tt">cab</span> and <span class="tex-font-style-tt">cba</span>.</p><p>Since you type your password with one finger, you need to spend time moving your finger from one password character to the next. The time to move from character $s_i$ to character $s_{i+1}$ is equal to the distance between these characters on keyboard. The total time you have to spend typing the password with a keyboard is called the <span class="tex-font-style-it">slowness</span> of this keyboard.</p><p>More formaly, the slowness of keyboard is equal to $\sum\limits_{i=2}^{n} |pos_{s_{i-1}} - pos_{s_i} |$, where $pos_x$ is position of letter $x$ in keyboard.</p><p>For example, if $s$ is <span class="tex-font-style-tt">aacabc</span> and the keyboard is <span class="tex-font-style-tt">bac</span>, then the total time of typing this password is $|pos_a - pos_a| + |pos_a - pos_c| + |pos_c - pos_a| + |pos_a - pos_b| + |pos_b - pos_c|$ = $|2 - 2| + |2 - 3| + |3 - 2| + |2 - 1| + |1 - 3|$ = $0 + 1 + 1 + 1 + 2 = 5$.</p><p>Before buying a new keyboard you want to know the minimum possible slowness that the keyboard can have. </p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^5, 1 \le m \le 20$).</p><p>The second line contains the string $s$ consisting of $n$ characters. Each character is one of the first $m$ Latin letters (lowercase).</p></div><div class="output-specification"><p>Print one integer – the minimum slowness a keyboard can have.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^5, 1 \le m \le 20$).</p><p>The second line contains the string $s$ consisting of $n$ characters. Each character is one of the first $m$ Latin letters (lowercase).</p>

## Output

<p>Print one integer – the minimum slowness a keyboard can have.</p>





```input1
6 3
aacabc
```




```input2
6 4
aaaaaa
```




```input3
15 4
abacabadabacaba
```




```output1
5
```




```output2
0
```




```output3
16
```



## Note

<p>The first test case is considered in the statement.</p><p>In the second test case the slowness of any keyboard is $0$.</p><p>In the third test case one of the most suitable keyboards is <span class="tex-font-style-tt">bacd</span>.</p>
