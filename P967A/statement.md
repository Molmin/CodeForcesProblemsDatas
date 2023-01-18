## Description

<div><p>These days Arkady works as an air traffic controller at a large airport. He controls a runway which is usually used for landings only. Thus, he has a schedule of planes that are landing in the nearest future, each landing lasts $1$ minute.</p><p>He was asked to insert one takeoff in the schedule. The takeoff takes $1$ minute itself, but for safety reasons there should be a time space between the takeoff and any landing of at least $s$ minutes from both sides.</p><p>Find the earliest time when Arkady can insert the takeoff.</p></div><div class="input-specification"><p>The first line of input contains two integers $n$ and $s$ ($1 \le n \le 100$, $1 \le s \le 60$)&nbsp;— the number of landings on the schedule and the minimum allowed time (in minutes) between a landing and a takeoff.</p><p>Each of next $n$ lines contains two integers $h$ and $m$ ($0 \le h \le 23$, $0 \le m \le 59$)&nbsp;— the time, in hours and minutes, when a plane will land, starting from current moment (i.&nbsp;e. the current time is $0$ $0$). These times are given in increasing order.</p></div><div class="output-specification"><p>Print two integers $h$ and $m$&nbsp;— the hour and the minute from the current moment of the earliest time Arkady can insert the takeoff.</p></div>

## Input

<p>The first line of input contains two integers $n$ and $s$ ($1 \le n \le 100$, $1 \le s \le 60$)&nbsp;— the number of landings on the schedule and the minimum allowed time (in minutes) between a landing and a takeoff.</p><p>Each of next $n$ lines contains two integers $h$ and $m$ ($0 \le h \le 23$, $0 \le m \le 59$)&nbsp;— the time, in hours and minutes, when a plane will land, starting from current moment (i.&nbsp;e. the current time is $0$ $0$). These times are given in increasing order.</p>

## Output

<p>Print two integers $h$ and $m$&nbsp;— the hour and the minute from the current moment of the earliest time Arkady can insert the takeoff.</p>





```input1
6 60
0 0
1 20
3 21
5 0
19 30
23 40

```




```input2
16 50
0 30
1 20
3 0
4 30
6 10
7 50
9 30
11 10
12 50
14 30
16 10
17 50
19 30
21 10
22 50
23 59

```




```input3
3 17
0 30
1 0
12 0

```




```output1
6 1

```




```output2
24 50

```




```output3
0 0

```



## Note

<p>In the first example note that there is not enough time between <span class="tex-font-style-tt">1:20</span> and <span class="tex-font-style-tt">3:21</span>, because each landing and the takeoff take one minute.</p><p>In the second example there is no gaps in the schedule, so Arkady can only add takeoff after all landings. Note that it is possible that one should wait more than $24$ hours to insert the takeoff.</p><p>In the third example Arkady can insert the takeoff even between the first landing.</p>
