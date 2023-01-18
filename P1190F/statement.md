## Description

<div><p>Tokitsukaze is playing a room escape game designed by SkywalkerT. In this game, she needs to find out hidden clues in the room to reveal a way to escape.</p><p>After a while, she realizes that the only way to run away is to open the digital door lock since she accidentally went into a secret compartment and found some clues, which can be interpreted as:</p><ul> <li> Only when you enter $n$ possible different passwords can you open the door; </li><li> Passwords must be integers ranged from $0$ to $(m - 1)$; </li><li> A password cannot be $x$ ($0 \leq x &lt; m$) if $x$ and $m$ are not <span class="tex-font-style-bf">coprime</span> (i.e. $x$ and $m$ have some common divisor greater than $1$); </li><li> A password cannot be $x$ ($0 \leq x &lt; m$) if there exist <span class="tex-font-style-bf">non-negative</span> integers $e$ and $k$ such that $p^e = k m + x$, where $p$ is a secret integer; </li><li> Any integer that doesn't break the above rules can be a password; </li><li> Several integers are hidden in the room, but only one of them can be $p$. </li></ul><p>Fortunately, she finds that $n$ and $m$ are recorded in the lock. However, what makes Tokitsukaze frustrated is that she doesn't do well in math. Now that she has found an integer that is suspected to be $p$, she wants you to help her find out $n$ possible passwords, or determine the integer cannot be $p$.</p></div><div class="input-specification"><p>The only line contains three integers $n$, $m$ and $p$ ($1 \leq n \leq 5 \times 10^5$, $1 \leq p &lt; m \leq 10^{18}$).</p><p>It is guaranteed that $m$ is <span class="tex-font-style-bf">a positive integer power of a single prime number.</span></p></div><div class="output-specification"><p>If the number of possible different passwords is less than $n$, print a single integer $-1$.</p><p>Otherwise, print $n$ distinct integers ranged from $0$ to $(m - 1)$ as passwords. You can print these integers in any order. Besides, if there are multiple solutions, print any.</p></div>

## Input

<p>The only line contains three integers $n$, $m$ and $p$ ($1 \leq n \leq 5 \times 10^5$, $1 \leq p &lt; m \leq 10^{18}$).</p><p>It is guaranteed that $m$ is <span class="tex-font-style-bf">a positive integer power of a single prime number.</span></p>

## Output

<p>If the number of possible different passwords is less than $n$, print a single integer $-1$.</p><p>Otherwise, print $n$ distinct integers ranged from $0$ to $(m - 1)$ as passwords. You can print these integers in any order. Besides, if there are multiple solutions, print any.</p>





```input1
1 2 1
```




```input2
3 5 1
```




```input3
2 5 4
```




```input4
4 9 8
```




```output1
-1
```




```output2
2 4 3
```




```output3
2 3
```




```output4
2 4 7 5
```



## Note

<p>In the first example, there is no possible password.</p><p>In each of the last three examples, the given integer $n$ equals to the number of possible different passwords for the given integers $m$ and $p$, so if the order of numbers in the output is ignored, the solution is unique as shown above.</p>
