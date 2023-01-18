## Description

<div><p>You successfully found poor Arkady near the exit of the station you've perfectly predicted. You sent him home on a taxi and suddenly came up with a question.</p><p>There are $n$ crossroads in your city and several bidirectional roads connecting some of them. A <span class="tex-font-style-it">taxi ride</span> is a path from some crossroads to another one without passing the same crossroads twice. You have a collection of rides made by one driver and now you wonder if this driver can be a robot or they are definitely a human.</p><p>You think that the driver can be a robot if for every two crossroads $a$ and $b$ the driver always chooses the same path whenever he drives from $a$ to $b$. Note that $a$ and $b$ here do not have to be the endpoints of a ride and that the path from $b$ to $a$ can be different. On the contrary, if the driver ever has driven two different paths from $a$ to $b$, they are definitely a human.</p><p>Given the system of roads and the description of all rides available to you, determine if the driver can be a robot or not.</p></div><div class="input-specification"><p>Each test contains one or more test cases. The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^5$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$)&nbsp;— the number of crossroads in the city.</p><p>The next line contains a single integer $q$ ($1 \le q \le 3 \cdot 10^5$)&nbsp;— the number of rides available to you.</p><p>Each of the following $q$ lines starts with a single integer $k$ ($2 \le k \le n$)&nbsp;— the number of crossroads visited by the driver on this ride. It is followed by $k$ integers $c_1$, $c_2$, ..., $c_k$ ($1 \le c_i \le n$)&nbsp;— the crossroads in the order the driver visited them. It is guaranteed that all crossroads in one ride are distinct.</p><p>It is guaranteed that the sum of values $k$ among all rides of all test cases does not exceed $3 \cdot 10^5$.</p><p>It is guaranteed that the sum of values $n$ and the sum of values $q$ doesn't exceed $3 \cdot 10^5$ among all test cases.</p></div><div class="output-specification"><p>Output a single line for each test case.</p><p>If the driver can be a robot, output "<span class="tex-font-style-tt">Robot</span>" in a single line. Otherwise, output "<span class="tex-font-style-tt">Human</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>Each test contains one or more test cases. The first line contains a single integer $t$ ($1 \le t \le 3 \cdot 10^5$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 3 \cdot 10^5$)&nbsp;— the number of crossroads in the city.</p><p>The next line contains a single integer $q$ ($1 \le q \le 3 \cdot 10^5$)&nbsp;— the number of rides available to you.</p><p>Each of the following $q$ lines starts with a single integer $k$ ($2 \le k \le n$)&nbsp;— the number of crossroads visited by the driver on this ride. It is followed by $k$ integers $c_1$, $c_2$, ..., $c_k$ ($1 \le c_i \le n$)&nbsp;— the crossroads in the order the driver visited them. It is guaranteed that all crossroads in one ride are distinct.</p><p>It is guaranteed that the sum of values $k$ among all rides of all test cases does not exceed $3 \cdot 10^5$.</p><p>It is guaranteed that the sum of values $n$ and the sum of values $q$ doesn't exceed $3 \cdot 10^5$ among all test cases.</p>

## Output

<p>Output a single line for each test case.</p><p>If the driver can be a robot, output "<span class="tex-font-style-tt">Robot</span>" in a single line. Otherwise, output "<span class="tex-font-style-tt">Human</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
1
5
2
4 1 2 3 5
3 1 4 3
```




```input2
1
4
4
3 1 2 3
3 2 3 4
3 3 4 1
3 4 1 2
```




```output1
Human
```




```output2
Robot
```



## Note

<p>In the first example it is clear that the driver used two different ways to get from crossroads $1$ to crossroads $3$. It must be a human.</p><p>In the second example the driver always drives the cycle $1 \to 2 \to 3 \to 4 \to 1$ until he reaches destination.</p>
