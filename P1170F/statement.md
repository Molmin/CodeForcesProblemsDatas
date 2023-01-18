## Description

<div><p>Polycarp has $n$ wheels and a car with $m$ slots for wheels. The initial pressure in the $i$-th wheel is $a_i$.</p><p>Polycarp's goal is to take <span class="tex-font-style-bf">exactly $m$ wheels</span> among the given $n$ wheels and equalize the pressure in them (then he can put these wheels in a car and use it for driving). In one minute he can decrease or increase the pressure in any (single) wheel by $1$. He can increase the pressure <span class="tex-font-style-bf">no more than $k$ times</span> in total because it is hard to pump up wheels.</p><p>Help Polycarp and say what is the minimum number of minutes he needs to spend to equalize the pressure of at least $m$ wheels among the given $n$ wheels.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n, m$ and $k$ ($1 \le m \le n \le 2 \cdot 10^5, 0 \le k \le 10^9$) — the number of wheels, the number of slots for wheels in a car and the number of times Polycarp can increase by $1$ the pressure in a wheel.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the pressure in the $i$-th wheel.</p></div><div class="output-specification"><p>Print one integer — the minimum number of minutes Polycarp needs to spend to equalize the pressure in at least $m$ wheels among the given $n$ wheels.</p></div>

## Input

<p>The first line of the input contains three integers $n, m$ and $k$ ($1 \le m \le n \le 2 \cdot 10^5, 0 \le k \le 10^9$) — the number of wheels, the number of slots for wheels in a car and the number of times Polycarp can increase by $1$ the pressure in a wheel.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the pressure in the $i$-th wheel.</p>

## Output

<p>Print one integer — the minimum number of minutes Polycarp needs to spend to equalize the pressure in at least $m$ wheels among the given $n$ wheels.</p>





```input1
6 6 7
6 15 16 20 1 5
```




```input2
6 3 1
4 8 15 16 23 42
```




```input3
5 4 0
5 5 5 4 5
```




```output1
39
```




```output2
8
```




```output3
0
```


