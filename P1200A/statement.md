## Description

<div><p>Amugae has a hotel consisting of $10$ rooms. The rooms are numbered from $0$ to $9$ from left to right.</p><p>The hotel has two entrances — one from the left end, and another from the right end. When a customer arrives to the hotel through the left entrance, they are assigned to an empty room closest to the left entrance. Similarly, when a customer arrives at the hotel through the right entrance, they are assigned to an empty room closest to the right entrance.</p><p>One day, Amugae lost the room assignment list. Thankfully Amugae's memory is perfect, and he remembers all of the customers: when a customer arrived, from which entrance, and when they left the hotel. Initially the hotel was empty. Write a program that recovers the room assignment list from Amugae's memory.</p></div><div class="input-specification"><p>The first line consists of an integer $n$ ($1 \le n \le 10^5$), the number of events in Amugae's memory.</p><p>The second line consists of a string of length $n$ describing the events in chronological order. Each character represents: </p><ul> <li> '<span class="tex-font-style-tt">L</span>': A customer arrives from the left entrance. </li><li> '<span class="tex-font-style-tt">R</span>': A customer arrives from the right entrance. </li><li> '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', ..., '<span class="tex-font-style-tt">9</span>': The customer in room $x$ ($0$, $1$, ..., $9$ respectively) leaves. </li></ul><p>It is guaranteed that there is at least one empty room when a customer arrives, and there is a customer in the room $x$ when $x$ ($0$, $1$, ..., $9$) is given. Also, all the rooms are initially empty.</p></div><div class="output-specification"><p>In the only line, output the hotel room's assignment status, from room $0$ to room $9$. Represent an empty room as '<span class="tex-font-style-tt">0</span>', and an occupied room as '<span class="tex-font-style-tt">1</span>', without spaces.</p></div>

## Input

<p>The first line consists of an integer $n$ ($1 \le n \le 10^5$), the number of events in Amugae's memory.</p><p>The second line consists of a string of length $n$ describing the events in chronological order. Each character represents: </p><ul> <li> '<span class="tex-font-style-tt">L</span>': A customer arrives from the left entrance. </li><li> '<span class="tex-font-style-tt">R</span>': A customer arrives from the right entrance. </li><li> '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">1</span>', ..., '<span class="tex-font-style-tt">9</span>': The customer in room $x$ ($0$, $1$, ..., $9$ respectively) leaves. </li></ul><p>It is guaranteed that there is at least one empty room when a customer arrives, and there is a customer in the room $x$ when $x$ ($0$, $1$, ..., $9$) is given. Also, all the rooms are initially empty.</p>

## Output

<p>In the only line, output the hotel room's assignment status, from room $0$ to room $9$. Represent an empty room as '<span class="tex-font-style-tt">0</span>', and an occupied room as '<span class="tex-font-style-tt">1</span>', without spaces.</p>





```input1
8
LLRL1RL1
```




```input2
9
L0L0LLRR9
```




```output1
1010000011
```




```output2
1100000010
```



## Note

<p>In the first example, hotel room's assignment status after each action is as follows. </p><ul> <li> First of all, all rooms are empty. Assignment status is <span class="tex-font-style-tt">0000000000</span>. </li><li> <span class="tex-font-style-tt">L</span>: a customer arrives to the hotel through the left entrance. Assignment status is <span class="tex-font-style-tt">1000000000</span>. </li><li> <span class="tex-font-style-tt">L</span>: one more customer from the left entrance. Assignment status is <span class="tex-font-style-tt">1100000000</span>. </li><li> <span class="tex-font-style-tt">R</span>: one more customer from the right entrance. Assignment status is <span class="tex-font-style-tt">1100000001</span>. </li><li> <span class="tex-font-style-tt">L</span>: one more customer from the left entrance. Assignment status is <span class="tex-font-style-tt">1110000001</span>. </li><li> <span class="tex-font-style-tt">1</span>: the customer in room $1$ leaves. Assignment status is <span class="tex-font-style-tt">1010000001</span>. </li><li> <span class="tex-font-style-tt">R</span>: one more customer from the right entrance. Assignment status is <span class="tex-font-style-tt">1010000011</span>. </li><li> <span class="tex-font-style-tt">L</span>: one more customer from the left entrance. Assignment status is <span class="tex-font-style-tt">1110000011</span>. </li><li> <span class="tex-font-style-tt">1</span>: the customer in room $1$ leaves. Assignment status is <span class="tex-font-style-tt">1010000011</span>. </li></ul><p>So after all, hotel room's final assignment status is <span class="tex-font-style-tt">1010000011</span>.</p><p>In the second example, hotel room's assignment status after each action is as follows. </p><ul> <li> <span class="tex-font-style-tt">L</span>: a customer arrives to the hotel through the left entrance. Assignment status is <span class="tex-font-style-tt">1000000000</span>. </li><li> <span class="tex-font-style-tt">0</span>: the customer in room $0$ leaves. Assignment status is <span class="tex-font-style-tt">0000000000</span>. </li><li> <span class="tex-font-style-tt">L</span>: a customer arrives to the hotel through the left entrance. Assignment status is <span class="tex-font-style-tt">1000000000</span> again. </li><li> <span class="tex-font-style-tt">0</span>: the customer in room $0$ leaves. Assignment status is <span class="tex-font-style-tt">0000000000</span>. </li><li> <span class="tex-font-style-tt">L</span>: a customer arrives to the hotel through the left entrance. Assignment status is <span class="tex-font-style-tt">1000000000</span>. </li><li> <span class="tex-font-style-tt">L</span>: one more customer from the left entrance. Assignment status is <span class="tex-font-style-tt">1100000000</span>. </li><li> <span class="tex-font-style-tt">R</span>: one more customer from the right entrance. Assignment status is <span class="tex-font-style-tt">1100000001</span>. </li><li> <span class="tex-font-style-tt">R</span>: one more customer from the right entrance. Assignment status is <span class="tex-font-style-tt">1100000011</span>. </li><li> <span class="tex-font-style-tt">9</span>: the customer in room $9$ leaves. Assignment status is <span class="tex-font-style-tt">1100000010</span>. </li></ul><p>So after all, hotel room's final assignment status is <span class="tex-font-style-tt">1100000010</span>.</p>
