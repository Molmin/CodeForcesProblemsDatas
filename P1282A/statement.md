## Description

<div><p>Polycarp lives on the coordinate axis $Ox$ and travels from the point $x=a$ to $x=b$. It moves uniformly rectilinearly at a speed of one unit of distance per minute.</p><p>On the axis $Ox$ at the point $x=c$ the base station of the mobile operator is placed. It is known that the radius of its coverage is $r$. Thus, if Polycarp is at a distance less than or equal to $r$ from the point $x=c$, then he is in the network coverage area, otherwise&nbsp;— no. The base station can be located both on the route of Polycarp and outside it.</p><p>Print the time in minutes during which Polycarp will <span class="tex-font-style-bf">not be</span> in the coverage area of the network, with a rectilinear uniform movement from $x=a$ to $x=b$. His speed&nbsp;— one unit of distance per minute.</p></div><div class="input-specification"><p>The first line contains a positive integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. In the following lines are written $t$ test cases.</p><p>The description of each test case is one line, which contains four integers $a$, $b$, $c$ and $r$ ($-10^8 \le a,b,c \le 10^8$, $0 \le r \le 10^8$)&nbsp;— the coordinates of the starting and ending points of the path, the base station, and its coverage radius, respectively.</p><p>Any of the numbers $a$, $b$ and $c$ can be equal (either any pair or all three numbers). The base station can be located both on the route of Polycarp and outside it.</p></div><div class="output-specification"><p>Print $t$ numbers&nbsp;— answers to given test cases in the order they are written in the test. Each answer is an integer&nbsp;— the number of minutes during which Polycarp will be <span class="tex-font-style-bf">unavailable</span> during his movement.</p></div>

## Input

<p>The first line contains a positive integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. In the following lines are written $t$ test cases.</p><p>The description of each test case is one line, which contains four integers $a$, $b$, $c$ and $r$ ($-10^8 \le a,b,c \le 10^8$, $0 \le r \le 10^8$)&nbsp;— the coordinates of the starting and ending points of the path, the base station, and its coverage radius, respectively.</p><p>Any of the numbers $a$, $b$ and $c$ can be equal (either any pair or all three numbers). The base station can be located both on the route of Polycarp and outside it.</p>

## Output

<p>Print $t$ numbers&nbsp;— answers to given test cases in the order they are written in the test. Each answer is an integer&nbsp;— the number of minutes during which Polycarp will be <span class="tex-font-style-bf">unavailable</span> during his movement.</p>





```input1
9
1 10 7 1
3 3 3 0
8 2 10 4
8 2 10 100
-10 20 -17 2
-3 2 2 0
-3 1 2 0
2 3 2 3
-1 3 -2 2
```




```output1
7
0
4
0
30
5
4
0
3
```



## Note

<p>The following picture illustrates the first test case. </p><center> <img class="tex-graphics" src="file://TuWmwWha.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">Polycarp goes from $1$ to $10$. The yellow area shows the coverage area of the station with a radius of coverage of $1$, which is located at the point of $7$. The green area shows a part of the path when Polycarp is out of coverage area.</span> </center>
