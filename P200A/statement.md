## Description

<div><p>The capital of Berland has the only movie theater in the country. Besides, it consists of only one room. The room is divided into <span class="tex-span"><i>n</i></span> rows, each row consists of <span class="tex-span"><i>m</i></span> seats.</p><p>There are <span class="tex-span"><i>k</i></span> people lined up to the box office, each person wants to buy exactly one ticket for his own entertainment. Before the box office started selling tickets, each person found the seat that seemed best for him and remembered it as a pair of coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the row number, and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> is the seat number in this row.</p><p>It is possible that some people have chosen the same place, then when some people see their favorite seat taken in the plan of empty seats in the theater, they choose and buy a ticket to another place. Each of them has the following logic: let's assume that he originally wanted to buy a ticket to seat <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">1</sub>)</span>, then when he comes to the box office, he chooses such empty seat <span class="tex-span">(<i>x</i><sub class="lower-index">2</sub>, <i>y</i><sub class="lower-index">2</sub>)</span>, which satisfies the following conditions: </p><ul> <li> the value of <span class="tex-span">|<i>x</i><sub class="lower-index">1</sub> - <i>x</i><sub class="lower-index">2</sub>| + |<i>y</i><sub class="lower-index">1</sub> - <i>y</i><sub class="lower-index">2</sub>|</span> is minimum </li><li> if the choice is not unique, then among the seats that satisfy the first condition, this person selects the one for which the value of <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> is minimum </li><li> if the choice is still not unique, among the seats that satisfy the first and second conditions, this person selects the one for which the value of <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> is minimum </li></ul><p>Your task is to find the coordinates of a seat for each person.</p></div><div class="input-specification"><p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 10<sup class="upper-index">5</sup></span>) — the number of rows in the room, the number of seats in each row and the number of people in the line, correspondingly. Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the coordinates of the seat each person has chosen. Numbers on the same line are separated by a space. The pairs of coordinates are located in the order, in which people stand in the line, starting from the head (the first person in the line who stands in front of the box office) to the tail (the last person in the line).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> lines, each containing a pair of integers. Print on the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the seat, for which the person who stands <span class="tex-span"><i>i</i></span>-th in the line will buy the ticket. </p></div>

## Input

<p>The first input line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>·<i>m</i>, 10<sup class="upper-index">5</sup></span>) — the number of rows in the room, the number of seats in each row and the number of people in the line, correspondingly. Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the coordinates of the seat each person has chosen. Numbers on the same line are separated by a space. The pairs of coordinates are located in the order, in which people stand in the line, starting from the head (the first person in the line who stands in front of the box office) to the tail (the last person in the line).</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> lines, each containing a pair of integers. Print on the <span class="tex-span"><i>i</i></span>-th line <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the seat, for which the person who stands <span class="tex-span"><i>i</i></span>-th in the line will buy the ticket. </p>





```input1
3 4 6
1 1
1 1
1 1
1 2
1 3
1 3

```




```input2
4 3 12
2 2
2 2
2 2
2 2
2 2
2 2
2 2
2 2
2 2
2 2
2 2
2 2

```




```output1
1 1
1 2
2 1
1 3
1 4
2 3

```




```output2
2 2
1 2
2 1
2 3
3 2
1 1
1 3
3 1
3 3
4 2
4 1
4 3

```


