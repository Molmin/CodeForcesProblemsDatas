## Description

<div><p>This time around, Baby Ehab will play with permutations. He has $n$ cubes arranged in a row, with numbers from $1$ to $n$ written on them. He'll make <span class="tex-font-style-bf">exactly</span> $j$ operations. In each operation, he'll pick up $2$ cubes and switch their positions.</p><p>He's wondering: how many different sequences of cubes can I have at the end? Since Baby Ehab is a turbulent person, he doesn't know how many operations he'll make, so he wants the answer for every possible $j$ between $1$ and $k$.</p></div><div class="input-specification"><p>The only line contains $2$ integers $n$ and $k$ ($2 \le n \le 10^9$, $1 \le k \le 200$)&nbsp;— the number of cubes Baby Ehab has, and the parameter $k$ from the statement.</p></div><div class="output-specification"><p>Print $k$ space-separated integers. The $i$-th of them is the number of possible sequences you can end up with if you do exactly $i$ operations. Since this number can be very large, print the remainder when it's divided by $10^9+7$.</p></div>

## Input

<p>The only line contains $2$ integers $n$ and $k$ ($2 \le n \le 10^9$, $1 \le k \le 200$)&nbsp;— the number of cubes Baby Ehab has, and the parameter $k$ from the statement.</p>

## Output

<p>Print $k$ space-separated integers. The $i$-th of them is the number of possible sequences you can end up with if you do exactly $i$ operations. Since this number can be very large, print the remainder when it's divided by $10^9+7$.</p>





```input1
2 3
```




```input2
3 2
```




```input3
4 2
```




```output1
1 1 1
```




```output2
3 3
```




```output3
6 12
```



## Note

<p>In the second example, there are $3$ sequences he can get after $1$ swap, because there are $3$ pairs of cubes he can swap. Also, there are $3$ sequences he can get after $2$ swaps:</p><ul> <li> $[1,2,3]$, </li><li> $[3,1,2]$, </li><li> $[2,3,1]$. </li></ul>
