## Description

<div><p>You are given two positive integers $x$ and $y$. You can perform the following operation with $x$: write it in its binary form without leading zeros, add $0$ or $1$ to the right of it, reverse the binary form and turn it into a decimal number which is assigned as the new value of $x$.</p><p>For example: </p><ul> <li> $34$ can be turned into $81$ via one operation: the binary form of $34$ is $100010$, if you add $1$, reverse it and remove leading zeros, you will get $1010001$, which is the binary form of $81$. </li><li> $34$ can be turned into $17$ via one operation: the binary form of $34$ is $100010$, if you add $0$, reverse it and remove leading zeros, you will get $10001$, which is the binary form of $17$. </li><li> $81$ can be turned into $69$ via one operation: the binary form of $81$ is $1010001$, if you add $0$, reverse it and remove leading zeros, you will get $1000101$, which is the binary form of $69$. </li><li> $34$ can be turned into $69$ via two operations: first you turn $34$ into $81$ and then $81$ into $69$. </li></ul><p>Your task is to find out whether $x$ can be turned into $y$ after a certain number of operations (possibly zero).</p></div><div class="input-specification"><p>The only line of the input contains two integers $x$ and $y$ ($1 \le x, y \le 10^{18}$).</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">YES</span> if you can make $x$ equal to $y$ and <span class="tex-font-style-tt">NO</span> if you can't.</p></div>

## Input

<p>The only line of the input contains two integers $x$ and $y$ ($1 \le x, y \le 10^{18}$).</p>

## Output

<p>Print <span class="tex-font-style-tt">YES</span> if you can make $x$ equal to $y$ and <span class="tex-font-style-tt">NO</span> if you can't.</p>





```input1
3 3
```




```input2
7 4
```




```input3
2 8
```




```input4
34 69
```




```input5
8935891487501725 71487131900013807
```




```output1
YES
```




```output2
NO
```




```output3
NO
```




```output4
YES
```




```output5
YES
```



## Note

<p>In the first example, you don't even need to do anything.</p><p>The fourth example is described in the statement.</p>
