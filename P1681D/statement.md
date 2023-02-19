## Description

<div><p>You are given two integer numbers, $n$ and $x$. You may perform several operations with the integer $x$.</p><p>Each operation you perform is the following one: choose any digit $y$ that occurs in the decimal representation of $x$ at least once, and replace $x$ by $x \cdot y$.</p><p>You want to make the length of decimal representation of $x$ (without leading zeroes) equal to $n$. What is the minimum number of operations required to do that?</p></div><div class="input-specification"><p>The only line of the input contains two integers $n$ and $x$ ($2 \le n \le 19$; $1 \le x &lt; 10^{n-1}$).</p></div><div class="output-specification"><p>Print one integer — the minimum number of operations required to make the length of decimal representation of $x$ (without leading zeroes) equal to $n$, or $-1$ if it is impossible.</p></div>

## Input

<p>The only line of the input contains two integers $n$ and $x$ ($2 \le n \le 19$; $1 \le x &lt; 10^{n-1}$).</p>

## Output

<p>Print one integer — the minimum number of operations required to make the length of decimal representation of $x$ (without leading zeroes) equal to $n$, or $-1$ if it is impossible.</p>





```input1
2 1
```




```input2
3 2
```




```input3
13 42
```




```output1
-1
```




```output2
4
```




```output3
12
```



## Note

<p>In the second example, the following sequence of operations achieves the goal:</p><ol> <li> multiply $x$ by $2$, so $x = 2 \cdot 2 = 4$; </li><li> multiply $x$ by $4$, so $x = 4 \cdot 4 = 16$; </li><li> multiply $x$ by $6$, so $x = 16 \cdot 6 = 96$; </li><li> multiply $x$ by $9$, so $x = 96 \cdot 9 = 864$. </li></ol>
