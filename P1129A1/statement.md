## Description

<div><p><span class="tex-font-style-bf"><span class="tex-font-style-it">This is a simplified version of the task Toy Train. These two versions differ only in the constraints. Hacks for this version are disabled.</span></span></p><p>Alice received a set of Toy Train™ from Bob. It consists of one train and a connected railway network of $n$ stations, enumerated from $1$ through $n$. The train occupies one station at a time and travels around the network of stations in a circular manner. More precisely, the immediate station that the train will visit after station $i$ is station $i+1$ if $1 \leq i &lt; n$ or station $1$ if $i = n$. It takes the train $1$ second to travel to its next station as described.</p><p>Bob gave Alice a fun task before he left: to deliver $m$ candies that are initially at some stations to their independent destinations using the train. The candies are enumerated from $1$ through $m$. Candy $i$ ($1 \leq i \leq m$), now at station $a_i$, should be delivered to station $b_i$ ($a_i \neq b_i$).</p><center> <img class="tex-graphics" src="file://SRyVpLN2.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The blue numbers on the candies correspond to $b_i$ values. The image corresponds to the $1$-st example.</span> </center><p>The train has infinite capacity, and it is possible to load off any number of candies at a station. However, only <span class="tex-font-style-bf">at most one</span> candy can be loaded from a station onto the train before it leaves the station. You can choose any candy at this station. The time it takes to move the candies is negligible.</p><p>Now, Alice wonders how much time is needed for the train to deliver all candies. Your task is to find, for each station, the minimum time the train would need to deliver all the candies were it to start from there.</p></div><div class="input-specification"><p>The first line contains two space-separated integers $n$ and $m$ ($2 \leq n \leq 100$; $1 \leq m \leq 200$) — the number of stations and the number of candies, respectively.</p><p>The $i$-th of the following $m$ lines contains two space-separated integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$; $a_i \neq b_i$) — the station that initially contains candy $i$ and the destination station of the candy, respectively.</p></div><div class="output-specification"><p>In the first and only line, print $n$ space-separated integers, the $i$-th of which is the minimum time, in seconds, the train would need to deliver all the candies were it to start from station $i$.</p></div>

## Input

<p>The first line contains two space-separated integers $n$ and $m$ ($2 \leq n \leq 100$; $1 \leq m \leq 200$) — the number of stations and the number of candies, respectively.</p><p>The $i$-th of the following $m$ lines contains two space-separated integers $a_i$ and $b_i$ ($1 \leq a_i, b_i \leq n$; $a_i \neq b_i$) — the station that initially contains candy $i$ and the destination station of the candy, respectively.</p>

## Output

<p>In the first and only line, print $n$ space-separated integers, the $i$-th of which is the minimum time, in seconds, the train would need to deliver all the candies were it to start from station $i$.</p>





```input1
5 7
2 4
5 1
2 3
3 4
4 1
5 3
3 5
```




```input2
2 3
1 2
1 2
1 2
```




```output1
10 9 10 10 9
```




```output2
5 6
```



## Note

<p>Consider the second sample.</p><p>If the train started at station $1$, the optimal strategy is as follows.</p><ol> <li> Load the first candy onto the train. </li><li> Proceed to station $2$. This step takes $1$ second. </li><li> Deliver the first candy. </li><li> Proceed to station $1$. This step takes $1$ second. </li><li> Load the second candy onto the train. </li><li> Proceed to station $2$. This step takes $1$ second. </li><li> Deliver the second candy. </li><li> Proceed to station $1$. This step takes $1$ second. </li><li> Load the third candy onto the train. </li><li> Proceed to station $2$. This step takes $1$ second. </li><li> Deliver the third candy. </li></ol><p>Hence, the train needs $5$ seconds to complete the tasks.</p><p>If the train were to start at station $2$, however, it would need to move to station $1$ before it could load the first candy, which would take one additional second. Thus, the answer in this scenario is $5+1 = 6$ seconds.</p>
