## Description

<div><p>Vasya likes to travel by train, but doesn't like when the car he travels in is located in the tail of the train.</p><p>Vasya gets on the train at the station. The train consists of $n$ cars indexed from $1$ to $n$ counting from the locomotive (head of the train). Three types of events occur while the train is moving:</p><ol> <li> Some number of cars are added to the head of the train; </li><li> Some number of cars are added to the tail of the train; </li><li> Vasya recalculates the values of the convenience of the cars (read more about it below). </li></ol><p>At each moment of time we will index the cars from the head of the train, starting from $1$. Note that when adding new cars to the head of the train, the indexing of the old ones may shift.</p><p>To choose which car to go in, Vasya will use the value $A_i$ for each car (where $i$ is a car index), which is calculated as follows:</p><ul> <li> At the beginning of the trip $A_i=0$, as well as for the new cars at the time of their addition. </li><li> During the next recalculation Vasya chooses some <span class="tex-font-style-bf">positive</span> integers $b$ and $s$ and adds to all $A_i$ value $b + (i - 1) \cdot s$. </li></ul><p>Vasya hasn't decided yet where he will get on the train and where will get off the train, so after each event of one of the three types he wants to know the least index of the car, such that its value $A_i$ is minimal. Since there is a lot of cars, Vasya asked you to write a program that answers his question.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 10^9$, $1 \leq m \leq 300\,000$), the number of cars in the train at the time of departure from the station and the number of stations, respectively.</p><p>Next $m$ lines contain the descriptions of events. Each event is one of the following three types:</p><ul> <li> "$1$ $k$" ($1 \le k \le 10^9$), add $k$ cars to the head of the train </li><li> "$2$ $k$" ($1 \le k \le 10^9$), add $k$ cars to the tail of the train </li><li> "$3$ $b$ $s$" ($1 \le b, s \le 10^9$), recalculate the convenience of all train cars. </li></ul><p>It is guaranteed that at any time the train length does not exceed $10^9$. Also it's guaranteed that the integers $A_i$ will not grow too high. Formally, it's guaranteed that if we sum the largest addition over all events of the $3$-rd type (that is, $b + (n - 1) \cdot s$, where $n$ is the number of cars at that moment) then the acquired sum would be at most $10^{18}$.</p></div><div class="output-specification"><p>After each of the $m$ queries print two integers: $j$ and $A_j$&nbsp;— the number of the car closest to the head of the train, such that its value $A_j$ is minimal, and the value $A_j$ itself.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \leq n \leq 10^9$, $1 \leq m \leq 300\,000$), the number of cars in the train at the time of departure from the station and the number of stations, respectively.</p><p>Next $m$ lines contain the descriptions of events. Each event is one of the following three types:</p><ul> <li> "$1$ $k$" ($1 \le k \le 10^9$), add $k$ cars to the head of the train </li><li> "$2$ $k$" ($1 \le k \le 10^9$), add $k$ cars to the tail of the train </li><li> "$3$ $b$ $s$" ($1 \le b, s \le 10^9$), recalculate the convenience of all train cars. </li></ul><p>It is guaranteed that at any time the train length does not exceed $10^9$. Also it's guaranteed that the integers $A_i$ will not grow too high. Formally, it's guaranteed that if we sum the largest addition over all events of the $3$-rd type (that is, $b + (n - 1) \cdot s$, where $n$ is the number of cars at that moment) then the acquired sum would be at most $10^{18}$.</p>

## Output

<p>After each of the $m$ queries print two integers: $j$ and $A_j$&nbsp;— the number of the car closest to the head of the train, such that its value $A_j$ is minimal, and the value $A_j$ itself.</p>





```input1
1 8
1 1
3 1 1
3 1 1
2 1
2 1
3 1 1
2 1
3 1 5
```




```output1
1 0
1 1
1 2
3 0
3 0
1 3
5 0
1 4
```



## Note

<ul> <li> Initially the train consists of one car with $A_1 = 0$, let's denote train as $[0]$ for simplicity.</li><li> After adding one car to the head, train is $[0, 0]$.</li><li> After recalculation of values with parameters $b=1, s=1$, train is $[1, 2]$.</li><li> After another recalculation of values with the parameters $b=1, s=1$, train is $[2, 4]$.</li><li> After adding one car to the end, train is $[2, 4, 0]$.</li><li> After another adding one car to the end, train is $[2, 4, 0, 0]$.</li><li> After recalculation of values with parameters $b=1$, $s=1$, train is $[3, 6, 3, 4]$.</li><li> After adding one car to the end, train is $[3, 6, 3, 4, 0]$.</li><li> After recalculation of values with parameters $b=1$, $s=5$, train is $[4, 12, 14, 20, 21]$.</li></ul>
