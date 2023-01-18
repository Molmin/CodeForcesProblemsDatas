## Description

<div><p>There is a robot staying at $X=0$ on the $Ox$ axis. He has to walk to $X=n$. You are controlling this robot and controlling how he goes. The robot has a battery and an accumulator with a solar panel.</p><p>The $i$-th segment of the path (from $X=i-1$ to $X=i$) can be exposed to sunlight or not. The array $s$ denotes which segments are exposed to sunlight: if segment $i$ is exposed, then $s_i = 1$, otherwise $s_i = 0$.</p><p>The robot has one battery of capacity $b$ and one accumulator of capacity $a$. For each segment, you should choose which type of energy storage robot will use to go to the next point (it can be either battery or accumulator). If the robot goes using the battery, the current charge of the battery is decreased by one (the robot can't use the battery if its charge is zero). And if the robot goes using the accumulator, the current charge of the accumulator is decreased by one (and the robot also can't use the accumulator if its charge is zero).</p><p>If the current segment is <span class="tex-font-style-bf">exposed to sunlight</span> and the robot goes through it <span class="tex-font-style-bf">using the battery</span>, the charge of the accumulator increases by one (of course, its charge can't become higher than it's maximum capacity).</p><p>If accumulator is used to pass some segment, its charge decreases by 1 no matter if the segment is exposed or not.</p><p>You understand that it is not always possible to walk to $X=n$. You want your robot to go as far as possible. Find the maximum number of segments of distance the robot can pass if you control him optimally.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n, b, a$ ($1 \le n, b, a \le 2 \cdot 10^5$) — the robot's destination point, the battery capacity and the accumulator capacity, respectively.</p><p>The second line of the input contains $n$ integers $s_1, s_2, \dots, s_n$ ($0 \le s_i \le 1$), where $s_i$ is $1$ if the $i$-th segment of distance is exposed to sunlight, and $0$ otherwise.</p></div><div class="output-specification"><p>Print one integer — the maximum number of segments the robot can pass if you control him optimally.</p></div>

## Input

<p>The first line of the input contains three integers $n, b, a$ ($1 \le n, b, a \le 2 \cdot 10^5$) — the robot's destination point, the battery capacity and the accumulator capacity, respectively.</p><p>The second line of the input contains $n$ integers $s_1, s_2, \dots, s_n$ ($0 \le s_i \le 1$), where $s_i$ is $1$ if the $i$-th segment of distance is exposed to sunlight, and $0$ otherwise.</p>

## Output

<p>Print one integer — the maximum number of segments the robot can pass if you control him optimally.</p>





```input1
5 2 1
0 1 0 1 0
```




```input2
6 2 1
1 0 0 1 0 1
```




```output1
5
```




```output2
3
```



## Note

<p>In the first example the robot can go through the first segment using the accumulator, and charge levels become $b=2$ and $a=0$. The second segment can be passed using the battery, and charge levels become $b=1$ and $a=1$. The third segment can be passed using the accumulator, and charge levels become $b=1$ and $a=0$. The fourth segment can be passed using the battery, and charge levels become $b=0$ and $a=1$. And the fifth segment can be passed using the accumulator.</p><p>In the second example the robot can go through the maximum number of segments using battery two times and accumulator one time in any order.</p>
