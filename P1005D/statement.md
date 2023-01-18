## Description

<div><p>Polycarp likes numbers that are divisible by 3.</p><p>He has a huge number $s$. Polycarp wants to cut from it the maximum number of numbers that are divisible by $3$. To do this, he makes an arbitrary number of vertical cuts between pairs of adjacent digits. As a result, after $m$ such cuts, there will be $m+1$ parts in total. Polycarp analyzes each of the obtained numbers and finds the number of those that are divisible by $3$.</p><p>For example, if the original number is $s=3121$, then Polycarp can cut it into three parts with two cuts: $3|1|21$. As a result, he will get two numbers that are divisible by $3$.</p><p>Polycarp can make an arbitrary number of vertical cuts, where each cut is made between a pair of adjacent digits. The resulting numbers cannot contain extra leading zeroes (that is, the number can begin with <span class="tex-font-style-tt">0</span> if and only if this number is exactly one character '<span class="tex-font-style-tt">0</span>'). For example, <span class="tex-font-style-tt">007</span>, <span class="tex-font-style-tt">01</span> and <span class="tex-font-style-tt">00099</span> are not valid numbers, but <span class="tex-font-style-tt">90</span>, <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">10001</span> are valid.</p><p>What is the maximum number of numbers divisible by $3$ that Polycarp can obtain?</p></div><div class="input-specification"><p>The first line of the input contains a positive integer $s$. The number of digits of the number $s$ is between $1$ and $2\cdot10^5$, inclusive. The first (leftmost) digit is not equal to <span class="tex-font-style-tt">0</span>.</p></div><div class="output-specification"><p>Print the maximum number of numbers divisible by $3$ that Polycarp can get by making vertical cuts in the given number $s$.</p></div>

## Input

<p>The first line of the input contains a positive integer $s$. The number of digits of the number $s$ is between $1$ and $2\cdot10^5$, inclusive. The first (leftmost) digit is not equal to <span class="tex-font-style-tt">0</span>.</p>

## Output

<p>Print the maximum number of numbers divisible by $3$ that Polycarp can get by making vertical cuts in the given number $s$.</p>





```input1
3121

```




```input2
6

```




```input3
1000000000000000000000000000000000

```




```input4
201920181

```




```output1
2

```




```output2
1

```




```output3
33

```




```output4
4

```



## Note

<p>In the first example, an example set of optimal cuts on the number is <span class="tex-font-style-tt">3|1|21</span>.</p><p>In the second example, you do not need to make any cuts. The specified number <span class="tex-font-style-tt">6</span> forms one number that is divisible by $3$.</p><p>In the third example, cuts must be made between each pair of digits. As a result, Polycarp gets one digit <span class="tex-font-style-tt">1</span> and $33$ digits <span class="tex-font-style-tt">0</span>. Each of the $33$ digits <span class="tex-font-style-tt">0</span> forms a number that is divisible by $3$.</p><p>In the fourth example, an example set of optimal cuts is <span class="tex-font-style-tt">2|0|1|9|201|81</span>. The numbers $0$, $9$, $201$ and $81$ are divisible by $3$.</p>
