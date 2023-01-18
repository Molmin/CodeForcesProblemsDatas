## Description

<div><p>Natasha was already going to fly back to Earth when she remembered that she needs to go to the Martian store to buy Martian souvenirs for her friends.</p><p>It is known, that the Martian year lasts $x_{max}$ months, month lasts $y_{max}$ days, day lasts $z_{max}$ seconds. Natasha also knows that this store works according to the following schedule: 2 months in a year were selected: $x_l$ and $x_r$ ($1\le x_l\le x_r\le x_{max}$), 2 days in a month: $y_l$ and $y_r$ ($1\le y_l\le y_r\le y_{max}$) and 2 seconds in a day: $z_l$ and $z_r$ ($1\le z_l\le z_r\le z_{max}$). The store works at all such moments (month $x$, day $y$, second $z$), when simultaneously $x_l\le x\le x_r$, $y_l\le y\le y_r$ and $z_l\le z\le z_r$.</p><p>Unfortunately, Natasha does not know the numbers $x_l,x_r,y_l,y_r,z_l,z_r$.</p><p>One Martian told Natasha: "I went to this store $(n+m)$ times. $n$ times of them it was opened, and $m$ times&nbsp;— closed." He also described his every trip to the store: the month, day, second of the trip and whether the store was open or closed at that moment.</p><p>Natasha can go to the store $k$ times. For each of them, determine whether the store at the time of the trip is open, closed, or this information is unknown.</p></div><div class="input-specification"><p>The first line contains $6$ integers $x_{max}$, $y_{max}$, $z_{max}$, $n$, $m$, $k$ ($1\le x_{max},y_{max},z_{max}\le 10^5$, $1\le n\le 10^5$, $0\le m\le 10^5$, $1\le k\le 10^5$)&nbsp;— number of months in a year, days in a month, seconds in a day, times when the store (according to a Martian) was opened, when it was closed and Natasha's queries.</p><p>The $i$-th of the next $n$ lines contains $3$ integers $x_i$, $y_i$, $z_i$ ($1\le x_i\le x_{max}$, $1\le y_i\le y_{max}$, $1\le z_i\le z_{max}$)&nbsp;— month, day and second of $i$-th time, when the store, according to the Martian, was opened.</p><p>The $i$-th of the next $m$ lines contains $3$ integers $x_i$, $y_i$, $z_i$ ($1\le x_i\le x_{max}$, $1\le y_i\le y_{max}$, $1\le z_i\le z_{max}$)&nbsp;— month, day and second of $i$-th time, when the store, according to the Martian, was closed.</p><p>The $i$-th of the next $k$ lines contains $3$ integers $x_i$, $y_i$, $z_i$ ($1\le x_i\le x_{max}$, $1\le y_i\le y_{max}$, $1\le z_i\le z_{max}$)&nbsp;— month, day and second of $i$-th Natasha's query.</p></div><div class="output-specification"><p>If the Martian was mistaken and his information about when the store is open and when it is closed is inconsistent, print a single line "<span class="tex-font-style-tt">INCORRECT</span>" (without quotes).</p><p>Otherwise, print the first line "<span class="tex-font-style-tt">CORRECT</span>" (without quotes). Next output $k$ lines: in $i$-th of them, output an answer to $i$-th Natasha's query: "<span class="tex-font-style-tt">OPEN</span>" (without quotes), if the store was opened at the moment of this query, "<span class="tex-font-style-tt">CLOSED</span>" (without quotes), if it was closed, or "<span class="tex-font-style-tt">UNKNOWN</span>" (without quotes), if this information can not be determined on the basis of available data.</p></div>

## Input

<p>The first line contains $6$ integers $x_{max}$, $y_{max}$, $z_{max}$, $n$, $m$, $k$ ($1\le x_{max},y_{max},z_{max}\le 10^5$, $1\le n\le 10^5$, $0\le m\le 10^5$, $1\le k\le 10^5$)&nbsp;— number of months in a year, days in a month, seconds in a day, times when the store (according to a Martian) was opened, when it was closed and Natasha's queries.</p><p>The $i$-th of the next $n$ lines contains $3$ integers $x_i$, $y_i$, $z_i$ ($1\le x_i\le x_{max}$, $1\le y_i\le y_{max}$, $1\le z_i\le z_{max}$)&nbsp;— month, day and second of $i$-th time, when the store, according to the Martian, was opened.</p><p>The $i$-th of the next $m$ lines contains $3$ integers $x_i$, $y_i$, $z_i$ ($1\le x_i\le x_{max}$, $1\le y_i\le y_{max}$, $1\le z_i\le z_{max}$)&nbsp;— month, day and second of $i$-th time, when the store, according to the Martian, was closed.</p><p>The $i$-th of the next $k$ lines contains $3$ integers $x_i$, $y_i$, $z_i$ ($1\le x_i\le x_{max}$, $1\le y_i\le y_{max}$, $1\le z_i\le z_{max}$)&nbsp;— month, day and second of $i$-th Natasha's query.</p>

## Output

<p>If the Martian was mistaken and his information about when the store is open and when it is closed is inconsistent, print a single line "<span class="tex-font-style-tt">INCORRECT</span>" (without quotes).</p><p>Otherwise, print the first line "<span class="tex-font-style-tt">CORRECT</span>" (without quotes). Next output $k$ lines: in $i$-th of them, output an answer to $i$-th Natasha's query: "<span class="tex-font-style-tt">OPEN</span>" (without quotes), if the store was opened at the moment of this query, "<span class="tex-font-style-tt">CLOSED</span>" (without quotes), if it was closed, or "<span class="tex-font-style-tt">UNKNOWN</span>" (without quotes), if this information can not be determined on the basis of available data.</p>





```input1
10 10 10 3 1 3
2 6 2
4 2 4
6 4 6
9 9 9
3 3 3
10 10 10
8 8 8

```




```input2
10 10 10 1 1 1
2 5 7
2 5 7
8 9 10

```




```output1
CORRECT
OPEN
CLOSED
UNKNOWN

```




```output2
INCORRECT

```



## Note

<p>Consider the first test case.</p><p>There are $10$ months in a year, $10$ days in a month, and $10$ seconds in a day.</p><p>The store was opened in $3$ moments:</p><ul><li> month $2$, day $6$, second $2$;</li><li> month $4$, day $2$, second $4$;</li><li> month $6$, day $4$, second $6$.</li></ul><p>The store was closed at the time: month $9$, day $9$, second $9$.</p><p>Queries:</p><ul><li> month $3$, day $3$, second $3$&nbsp;— open ("<span class="tex-font-style-tt">OPEN</span>") (since the store opens no later than month $2$, day $2$, second $2$ and closes no earlier than in month $6$, day $6$, second $6$); </li><li> month $10$, day $10$, second $10$&nbsp;— closed ("<span class="tex-font-style-tt">CLOSED</span>") (since it is closed even in the month $9$, day $9$, second $9$);</li><li> month $8$, day $8$, second $8$&nbsp;— unknown ("<span class="tex-font-style-tt">UNKNOWN</span>") (because the schedule in which the store is open at this moment exists, and the schedule in which the store is closed at this moment exists as well).</li></ul><p>In the second test case, the store was closed and opened at the same time&nbsp;— contradiction ("<span class="tex-font-style-tt">INCORRECT</span>").</p>
