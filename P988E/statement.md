## Description

<div><p>You are given an integer $n$ from $1$ to $10^{18}$ without leading zeroes.</p><p>In one move you can swap any two adjacent digits in the given number in such a way that the resulting number will not contain leading zeroes. In other words, <span class="tex-font-style-bf">after each move</span> the number you have cannot contain any leading zeroes.</p><p>What is the minimum number of moves you have to make to obtain a number that is divisible by $25$? Print <span class="tex-font-style-tt">-1</span> if it is impossible to obtain a number that is divisible by $25$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 10^{18}$). It is guaranteed that the first (left) digit of the number $n$ is not a zero.</p></div><div class="output-specification"><p>If it is impossible to obtain a number that is divisible by $25$, print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum number of moves required to obtain such number.</p><p>Note that you can swap only adjacent digits in the given number.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 10^{18}$). It is guaranteed that the first (left) digit of the number $n$ is not a zero.</p>

## Output

<p>If it is impossible to obtain a number that is divisible by $25$, print <span class="tex-font-style-tt">-1</span>. Otherwise print the minimum number of moves required to obtain such number.</p><p>Note that you can swap only adjacent digits in the given number.</p>





```input1
5071

```




```input2
705

```




```input3
1241367

```




```output1
4

```




```output2
1

```




```output3
-1

```



## Note

<p>In the first example one of the possible sequences of moves is <span class="tex-font-style-tt">5071</span> $\rightarrow$ <span class="tex-font-style-tt">5701</span> $\rightarrow$ <span class="tex-font-style-tt">7501</span> $\rightarrow$ <span class="tex-font-style-tt">7510</span> $\rightarrow$ <span class="tex-font-style-tt">7150</span>.</p>
