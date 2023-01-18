## Description

<div><p>Vova's house is an array consisting of $n$ elements (yeah, this is the first problem, I think, where someone <span class="tex-font-style-it">lives</span> in the array). There are heaters in some positions of the array. The $i$-th element of the array is $1$ if there is a heater in the position $i$, otherwise the $i$-th element of the array is $0$.</p><p>Each heater has a value $r$ ($r$ is the same for all heaters). This value means that the heater at the position $pos$ can warm up all the elements in range $[pos - r + 1; pos + r - 1]$.</p><p>Vova likes to walk through his house while he thinks, and he hates cold positions of his house. Vova wants to switch some of his heaters on in such a way that each element of his house will be warmed up by at least one heater. </p><p>Vova's target is to warm up the whole house (all the elements of the array), i.e. if $n = 6$, $r = 2$ and heaters are at positions $2$ and $5$, then Vova can warm up the whole house if he switches all the heaters in the house on (then the first $3$ elements will be warmed up by the first heater and the last $3$ elements will be warmed up by the second heater).</p><p>Initially, all the heaters are off.</p><p>But from the other hand, Vova didn't like to pay much for the electricity. So he wants to switch the <span class="tex-font-style-bf">minimum</span> number of heaters on in such a way that each element of his house is warmed up by at least one heater.</p><p>Your task is to find this number of heaters or say that it is impossible to warm up the whole house.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $r$ ($1 \le n, r \le 1000$) — the number of elements in the array and the value of heaters.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 1$) — the Vova's house description.</p></div><div class="output-specification"><p>Print one integer — the minimum number of heaters needed to warm up the whole house or <span class="tex-font-style-tt">-1</span> if it is impossible to do it.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $r$ ($1 \le n, r \le 1000$) — the number of elements in the array and the value of heaters.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($0 \le a_i \le 1$) — the Vova's house description.</p>

## Output

<p>Print one integer — the minimum number of heaters needed to warm up the whole house or <span class="tex-font-style-tt">-1</span> if it is impossible to do it.</p>





```input1
6 2
0 1 1 0 0 1

```




```input2
5 3
1 0 0 0 1

```




```input3
5 10
0 0 0 0 0

```




```input4
10 3
0 0 1 1 0 1 0 0 0 1

```




```output1
3

```




```output2
2

```




```output3
-1

```




```output4
3

```



## Note

<p>In the first example the heater at the position $2$ warms up elements $[1; 3]$, the heater at the position $3$ warms up elements $[2, 4]$ and the heater at the position $6$ warms up elements $[5; 6]$ so the answer is $3$.</p><p>In the second example the heater at the position $1$ warms up elements $[1; 3]$ and the heater at the position $5$ warms up elements $[3; 5]$ so the answer is $2$.</p><p>In the third example there are no heaters so the answer is <span class="tex-font-style-tt">-1</span>.</p><p>In the fourth example the heater at the position $3$ warms up elements $[1; 5]$, the heater at the position $6$ warms up elements $[4; 8]$ and the heater at the position $10$ warms up elements $[8; 10]$ so the answer is $3$.</p>
