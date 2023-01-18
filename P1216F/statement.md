## Description

<div><p>You work as a system administrator in a dormitory, which has $n$ rooms one after another along a straight hallway. Rooms are numbered from $1$ to $n$.</p><p>You have to connect all $n$ rooms to the Internet.</p><p>You can connect each room to the Internet directly, the cost of such connection for the $i$-th room is $i$ coins. </p><p>Some rooms also have a spot for a router. The cost of placing a router in the $i$-th room is also $i$ coins. You cannot place a router in a room which does not have a spot for it. When you place a router in the room $i$, you connect all rooms with the numbers from $max(1,~i - k)$ to $min(n,~i + k)$ inclusive to the Internet, where $k$ is the range of router. The value of $k$ is the same for all routers. </p><p>Calculate the minimum total cost of connecting all $n$ rooms to the Internet. You can assume that the number of rooms which have a spot for a router is not greater than the number of routers you have.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n, k \le 2 \cdot 10^5$) — the number of rooms and the range of each router.</p><p>The second line of the input contains one string $s$ of length $n$, consisting only of zeros and ones. If the $i$-th character of the string equals to '<span class="tex-font-style-tt">1</span>' then there is a spot for a router in the $i$-th room. If the $i$-th character of the string equals to '<span class="tex-font-style-tt">0</span>' then you cannot place a router in the $i$-th room.</p></div><div class="output-specification"><p>Print one integer — the minimum total cost of connecting all $n$ rooms to the Internet.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n, k \le 2 \cdot 10^5$) — the number of rooms and the range of each router.</p><p>The second line of the input contains one string $s$ of length $n$, consisting only of zeros and ones. If the $i$-th character of the string equals to '<span class="tex-font-style-tt">1</span>' then there is a spot for a router in the $i$-th room. If the $i$-th character of the string equals to '<span class="tex-font-style-tt">0</span>' then you cannot place a router in the $i$-th room.</p>

## Output

<p>Print one integer — the minimum total cost of connecting all $n$ rooms to the Internet.</p>





```input1
5 2
00100
```




```input2
6 1
000000
```




```input3
4 1
0011
```




```input4
12 6
000010000100
```




```output1
3
```




```output2
21
```




```output3
4
```




```output4
15
```



## Note

<p>In the first example it is enough to place the router in the room $3$, then all rooms will be connected to the Internet. The total cost of connection is $3$.</p><p>In the second example you can place routers nowhere, so you need to connect all rooms directly. Thus, the total cost of connection of all rooms is $1 + 2 + 3 + 4 + 5 + 6 = 21$.</p><p>In the third example you need to connect the room $1$ directly and place the router in the room $3$. Thus, the total cost of connection of all rooms is $1 + 3 = 4$.</p><p>In the fourth example you need to place routers in rooms $5$ and $10$. Then all rooms will be connected to the Internet. The total cost of connection is $5 + 10 = 15$.</p>
