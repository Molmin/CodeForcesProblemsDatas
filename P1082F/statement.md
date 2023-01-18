## Description

<div><p>Polycarp's phone book contains $n$ phone numbers, each of them is described by $s_i$ — the number itself and $m_i$ — the number of times Polycarp dials it in daily.</p><p>Polycarp has just bought a brand new phone with an amazing <span class="tex-font-style-it">speed dial</span> feature! More precisely, $k$ buttons on it can have a number assigned to it (not necessary from the phone book). To enter some number Polycarp can press one of these $k$ buttons and then finish the number using usual digit buttons (entering a number with only digit buttons is also possible).</p><p><span class="tex-font-style-it">Speed dial</span> button can only be used when no digits are entered. No button can have its number reassigned.</p><p>What is the minimal total number of <span class="tex-font-style-bf">digit number presses</span> Polycarp can achieve after he assigns numbers to <span class="tex-font-style-it">speed dial</span> buttons and enters each of the numbers from his phone book the given number of times in an optimal way?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 500$, $1 \le k \le 10$) — the amount of numbers in Polycarp's phone book and the number of <span class="tex-font-style-it">speed dial</span> buttons his new phone has.</p><p>The $i$-th of the next $n$ lines contain a string $s_i$ and an integer $m_i$ $(1 \le m_i \le 500)$, where $s_i$ is a non-empty string of digits from $0$ to $9$ inclusive (the $i$-th number), and $m_i$ is the amount of times it will be dialed, respectively.</p><p>It is guaranteed that the total length of all phone numbers will not exceed $500$.</p></div><div class="output-specification"><p>Print a single integer — the minimal total number of <span class="tex-font-style-bf">digit number presses</span> Polycarp can achieve after he assigns numbers to <span class="tex-font-style-it">speed dial</span> buttons and enters each of the numbers from his phone book the given number of times in an optimal way.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 500$, $1 \le k \le 10$) — the amount of numbers in Polycarp's phone book and the number of <span class="tex-font-style-it">speed dial</span> buttons his new phone has.</p><p>The $i$-th of the next $n$ lines contain a string $s_i$ and an integer $m_i$ $(1 \le m_i \le 500)$, where $s_i$ is a non-empty string of digits from $0$ to $9$ inclusive (the $i$-th number), and $m_i$ is the amount of times it will be dialed, respectively.</p><p>It is guaranteed that the total length of all phone numbers will not exceed $500$.</p>

## Output

<p>Print a single integer — the minimal total number of <span class="tex-font-style-bf">digit number presses</span> Polycarp can achieve after he assigns numbers to <span class="tex-font-style-it">speed dial</span> buttons and enters each of the numbers from his phone book the given number of times in an optimal way.</p>





```input1
3 1
0001 5
001 4
01 1
```




```input2
3 1
0001 5
001 6
01 1
```




```output1
14
```




```output2
18
```



## Note

<p>The only <span class="tex-font-style-it">speed dial</span> button in the first example should have "<span class="tex-font-style-tt">0001</span>" on it. The total number of digit button presses will be $0 \cdot 5$ for the first number + $3 \cdot 4$ for the second + $2 \cdot 1$ for the third. $14$ in total.</p><p>The only <span class="tex-font-style-it">speed dial</span> button in the second example should have "<span class="tex-font-style-tt">00</span>" on it. The total number of digit button presses will be $2 \cdot 5$ for the first number + $1 \cdot 6$ for the second + $2 \cdot 1$ for the third. $18$ in total.</p>
