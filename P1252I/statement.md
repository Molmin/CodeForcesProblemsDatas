## Description

<div><p>Allen, a government secret service, has been assigned to infiltrate a mafia secret base to uncover crucial information regarding the mafia's operations.</p><p>The secret base is a rectangular bounded by $(x_L,y_L)$, $(x_L,y_R)$, $(x_R,y_L)$, and $(x_R,y_R)$ in a Cartesian coordinate system where $x_L &lt; x_R$ and $y_L &lt; y_R$. There are $N$ sensors placed inside the secret base. The $i^{th}$ sensor is located at $(x_i, y_i)$ and has an effective sensing radius of $r_i$ which can detect any person who is <span class="tex-font-style-bf">strictly</span> within the radius of $r_i$ from $(x_i, y_i)$. In other words, the $i^{th}$ sensor can detect a person at location $(x_a, y_a)$ if and only if the Euclidean distance of $(x_i, y_i)$ and $(x_a, y_a)$ is strictly less than $r_i$. It is also known that the Euclidean distance of any two sensors $i$ and $j$ is strictly larger than $r_i + r_j$. Note that the Euclidean distance of two points, $(x_a, y_a)$ and $(x_b, y_b)$, is $\sqrt{|x_a - x_b|^2 + |y_a - y_b|^2}$.</p><p>Allen begins his infiltration mission at location $(x_s, y_s)$, and his target is located at $(x_t, y_t)$. Allen has the power to run extremely fast in a straight line while he needs to spend extra time to change his running trajectory (to adjust his footing). Although he is a fast runner, he still needs to make sure that none of the sensors detect him while he is running, i.e. there is no point in his running trajectory which is strictly within a sensor effective sensing radius.</p><p>Let $P = \{(x_{p_1}, y_{p_1}), \dots, (x_{p_{|P|}}, y_{p_{|P|}})\}$ be the set of locations where Allen changes his running trajectory, thus, Allen's running trajectory with $P$ is $(x_s, y_s) \rightarrow (x_{p_1}, y_{p_1}) \rightarrow \dots \rightarrow (x_{p_{|P|}}, y_{p_{|P|}}) \rightarrow (x_t, y_t)$ where $(x_a,y_a) \rightarrow (x_b,y_b)$ implies that Allen is running from $(x_a,y_a)$ to $(x_b,y_b)$ in a straight line. The set $P$ is feasible if and only if with $P$, Allen is not detected by any sensor and is not running out of the secret base (although, Allen is allowed to run along the secret base perimeter). Note that $x_p$ and $y_p$, $(x_p,y_p) \in P$, are not necessarily integers; they can be <span class="tex-font-style-bf">real numbers</span>.</p><p>Your task in this problem is to find any one feasible $P$ which contains no more than $1000$ points.</p></div><div class="input-specification"><p>Input begins with a line containing five integers: $N$ $x_L$ $y_L$ $x_R$ $y_R$ ($0 \le N \le 50$; $0 \le x_L &lt; x_R \le 1000$; $0 \le y_L &lt; y_R \le 1000$) representing the number of sensors and the secret base ($x_L$, $y_L$, $x_R$, $y_R$), respectively. The next line contains two integers: $x_s$ $y_s$ ($x_L &lt; x_s &lt; x_R$; $y_L &lt; y_s &lt; y_R$) representing Allen's initial location. The next line contains two integers: $x_t$ $y_t$ ($x_L &lt; x_t &lt; x_R$; $y_L &lt; y_t &lt; y_R$) representing Allen's target location. It is guaranteed that $x_s \ne x_t$ or $y_s \ne y_t$. The next $N$ lines each contains three integers: $x_i$ $y_i$ $r_i$ ($x_L &lt; x_i - r_i &lt; x_i + r_i &lt; x_R$; $y_L &lt; y_i - r_i &lt; y_i + r_i &lt; y_R$; $1 \le r_i \le 1000$) representing a sensor at location $(x_i, y_i)$ with an effective sensing radius of $r_i$. It is guaranteed that the Euclidean distance of any two sensors $i$ and $j$ is larger than $r_i + r_j$. It is also guaranteed that the Euclidean distance of $(x_s,y_s)$ and $(x_t,y_t)$ to any sensor $i$ is larger than $r_i$.</p></div><div class="output-specification"><p>Output in a line an integer representing the size of a feasible $P$. The next $|P|$ lines each contains two real numbers (separated by a single space); the $j^{th}$ line contains $x_j$ $y_j$ representing the $j^{th}$ point in $P$. You may output any feasible $P$ with no more than $1000$ points.</p><p>Due to the nature of the output (floating point), let us define an epsilon $\epsilon$ to be $10^{-6}$ to verify the output. Consider $Q_1 = (x_s, y_s)$, $Q_{j+1} = P_j$ for all $1 \le j \le |P|$, and $Q_{|P|+2} = (x_t, y_t)$. Then, $P$ is considered correct if and only if $P$ contains no more than $1000$ points and all of the following are satisfied: </p><ul> <li> $x_L - \epsilon \le x_{p_k} \le x_R + \epsilon$ and $y_L - \epsilon \le y_{p_k} \le y_R + \epsilon$ for all $1 \le k \le |P|$ (Allen is not running out of the secret base). </li><li> For all $1 \le k &lt; |Q|$, let $S_k$ be the line segment connecting $Q_k$ and $Q_{k+1}$ (Allen is running in straight line). For all $1 \le i \le N$, let $(x_{k,i},y_{k,i})$ be the point along $S_k$ that is the closest to the $i^{th}$ sensor's location, $(x_i,y_i)$. Let $d_{k,i}$ be the Euclidean distance between $(x_{k,i},y_{k,i})$ and $(x_i,y_i)$. Then, the constraint $r_i \le d_{k,i} + \epsilon$ should be satisfied (Allen is not detected by any sensor). </li><li> All points in $Q$ are distinct. Two points, $(x_a,y_a)$ and $(x_b,y_b)$, are considered distinct if and only if $|x_a - x_b| &gt; \epsilon$ or $|y_a - y_b| &gt; \epsilon$. </li></ul></div>

## Input

<p>Input begins with a line containing five integers: $N$ $x_L$ $y_L$ $x_R$ $y_R$ ($0 \le N \le 50$; $0 \le x_L &lt; x_R \le 1000$; $0 \le y_L &lt; y_R \le 1000$) representing the number of sensors and the secret base ($x_L$, $y_L$, $x_R$, $y_R$), respectively. The next line contains two integers: $x_s$ $y_s$ ($x_L &lt; x_s &lt; x_R$; $y_L &lt; y_s &lt; y_R$) representing Allen's initial location. The next line contains two integers: $x_t$ $y_t$ ($x_L &lt; x_t &lt; x_R$; $y_L &lt; y_t &lt; y_R$) representing Allen's target location. It is guaranteed that $x_s \ne x_t$ or $y_s \ne y_t$. The next $N$ lines each contains three integers: $x_i$ $y_i$ $r_i$ ($x_L &lt; x_i - r_i &lt; x_i + r_i &lt; x_R$; $y_L &lt; y_i - r_i &lt; y_i + r_i &lt; y_R$; $1 \le r_i \le 1000$) representing a sensor at location $(x_i, y_i)$ with an effective sensing radius of $r_i$. It is guaranteed that the Euclidean distance of any two sensors $i$ and $j$ is larger than $r_i + r_j$. It is also guaranteed that the Euclidean distance of $(x_s,y_s)$ and $(x_t,y_t)$ to any sensor $i$ is larger than $r_i$.</p>

## Output

<p>Output in a line an integer representing the size of a feasible $P$. The next $|P|$ lines each contains two real numbers (separated by a single space); the $j^{th}$ line contains $x_j$ $y_j$ representing the $j^{th}$ point in $P$. You may output any feasible $P$ with no more than $1000$ points.</p><p>Due to the nature of the output (floating point), let us define an epsilon $\epsilon$ to be $10^{-6}$ to verify the output. Consider $Q_1 = (x_s, y_s)$, $Q_{j+1} = P_j$ for all $1 \le j \le |P|$, and $Q_{|P|+2} = (x_t, y_t)$. Then, $P$ is considered correct if and only if $P$ contains no more than $1000$ points and all of the following are satisfied: </p><ul> <li> $x_L - \epsilon \le x_{p_k} \le x_R + \epsilon$ and $y_L - \epsilon \le y_{p_k} \le y_R + \epsilon$ for all $1 \le k \le |P|$ (Allen is not running out of the secret base). </li><li> For all $1 \le k &lt; |Q|$, let $S_k$ be the line segment connecting $Q_k$ and $Q_{k+1}$ (Allen is running in straight line). For all $1 \le i \le N$, let $(x_{k,i},y_{k,i})$ be the point along $S_k$ that is the closest to the $i^{th}$ sensor's location, $(x_i,y_i)$. Let $d_{k,i}$ be the Euclidean distance between $(x_{k,i},y_{k,i})$ and $(x_i,y_i)$. Then, the constraint $r_i \le d_{k,i} + \epsilon$ should be satisfied (Allen is not detected by any sensor). </li><li> All points in $Q$ are distinct. Two points, $(x_a,y_a)$ and $(x_b,y_b)$, are considered distinct if and only if $|x_a - x_b| &gt; \epsilon$ or $|y_a - y_b| &gt; \epsilon$. </li></ul>





```input1
3 2 2 50 26
4 14
48 14
15 13 7
36 16 6
46 18 3
```




```input2
1 0 0 1000 1000
100 501
900 501
500 251 250
```




```output1
2
13.25 23.1234567
36.591003 7.1
```




```output2
0
```



## Note

<p><span class="tex-font-style-it">Explanation for the sample input/output #1</span></p><p><img class="tex-graphics" src="file://1CSCXsVs.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The figure above shows the $P$ from the sample output. Note that there exists a feasible $P$ with only one point in this sample, although you are not required to find such $P$.</p>
