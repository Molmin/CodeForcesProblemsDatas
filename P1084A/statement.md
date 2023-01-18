## Description

<div><p>The Fair Nut lives in $n$ story house. $a_i$ people live on the $i$-th floor of the house. Every person uses elevator twice a day: to get from the floor where he/she lives to the ground (first) floor and to get from the first floor to the floor where he/she lives, when he/she comes back home in the evening. </p><p>It was decided that elevator, when it is not used, will stay on the $x$-th floor, but $x$ hasn't been chosen yet. When a person needs to get from floor $a$ to floor $b$, elevator follows the simple algorithm: </p><ul> <li> Moves from the $x$-th floor (initially it stays on the $x$-th floor) to the $a$-th and takes the passenger. </li><li> Moves from the $a$-th floor to the $b$-th floor and lets out the passenger (if $a$ equals $b$, elevator just opens and closes the doors, <span class="tex-font-style-bf">but still</span> comes to the floor from the $x$-th floor). </li><li> Moves from the $b$-th floor back to the $x$-th. </li></ul> The elevator never transposes more than one person and always goes back to the floor $x$ before transposing a next passenger. The elevator spends one unit of electricity to move between neighboring floors. So moving from the $a$-th floor to the $b$-th floor requires $|a - b|$ units of electricity.<p>Your task is to help Nut to find the minimum number of electricity units, that it would be enough for one day, by choosing an optimal the $x$-th floor. Don't forget than elevator initially stays on the $x$-th floor. </p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of floors.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 100$)&nbsp;— the number of people on each floor.</p></div><div class="output-specification"><p>In a single line, print the answer to the problem&nbsp;— the minimum number of electricity units.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 100$)&nbsp;— the number of floors.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_i \leq 100$)&nbsp;— the number of people on each floor.</p>

## Output

<p>In a single line, print the answer to the problem&nbsp;— the minimum number of electricity units.</p>





```input1
3
0 2 1

```




```input2
2
1 1

```




```output1
16
```




```output2
4
```



## Note

<p>In the first example, the answer can be achieved by choosing the second floor as the $x$-th floor. Each person from the second floor (there are two of them) would spend $4$ units of electricity per day ($2$ to get down and $2$ to get up), and one person from the third would spend $8$ units of electricity per day ($4$ to get down and $4$ to get up). $4 \cdot 2 + 8 \cdot 1 = 16$.</p><p>In the second example, the answer can be achieved by choosing the first floor as the $x$-th floor.</p>
