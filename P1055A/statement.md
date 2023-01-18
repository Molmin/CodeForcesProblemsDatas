## Description

<div><p>Alice has a birthday today, so she invited home her best friend Bob. Now Bob needs to find a way to commute to the Alice's home.</p><p>In the city in which Alice and Bob live, the first metro line is being built. This metro line contains $n$ stations numbered from $1$ to $n$. Bob lives near the station with number $1$, while Alice lives near the station with number $s$. The metro line has two tracks. Trains on the first track go from the station $1$ to the station $n$ and trains on the second track go in reverse direction. Just after the train arrives to the end of its track, it goes to the depot immediately, so it is impossible to travel on it after that.</p><p>Some stations are not yet open at all and some are only partially open&nbsp;— for each station and for each track it is known whether the station is closed for that track or not. If a station is closed for some track, all trains going in this track's direction pass the station without stopping on it.</p><p>When the Bob got the information on opened and closed stations, he found that traveling by metro may be unexpectedly complicated. Help Bob determine whether he can travel to the Alice's home by metro or he should search for some other transport.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $s$ ($2 \le s \le n \le 1000$)&nbsp;— the number of stations in the metro and the number of the station where Alice's home is located. Bob lives at station $1$.</p><p>Next lines describe information about closed and open stations.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i = 0$ or $a_i = 1$). If $a_i = 1$, then the $i$-th station is open on the first track (that is, in the direction of increasing station numbers). Otherwise the station is closed on the first track.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($b_i = 0$ or $b_i = 1$). If $b_i = 1$, then the $i$-th station is open on the second track (that is, in the direction of decreasing station numbers). Otherwise the station is closed on the second track.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity) if Bob will be able to commute to the Alice's home by metro and "<span class="tex-font-style-tt">NO</span>" (quotes for clarity) otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains two integers $n$ and $s$ ($2 \le s \le n \le 1000$)&nbsp;— the number of stations in the metro and the number of the station where Alice's home is located. Bob lives at station $1$.</p><p>Next lines describe information about closed and open stations.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($a_i = 0$ or $a_i = 1$). If $a_i = 1$, then the $i$-th station is open on the first track (that is, in the direction of increasing station numbers). Otherwise the station is closed on the first track.</p><p>The third line contains $n$ integers $b_1, b_2, \ldots, b_n$ ($b_i = 0$ or $b_i = 1$). If $b_i = 1$, then the $i$-th station is open on the second track (that is, in the direction of decreasing station numbers). Otherwise the station is closed on the second track.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity) if Bob will be able to commute to the Alice's home by metro and "<span class="tex-font-style-tt">NO</span>" (quotes for clarity) otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
5 3
1 1 1 1 1
1 1 1 1 1

```




```input2
5 4
1 0 0 0 1
0 1 1 1 1

```




```input3
5 2
0 1 1 1 1
1 1 1 1 1

```




```output1
YES

```




```output2
YES

```




```output3
NO

```



## Note

<p>In the first example, all stations are opened, so Bob can simply travel to the station with number $3$.</p><p>In the second example, Bob should travel to the station $5$ first, switch to the second track and travel to the station $4$ then.</p><p>In the third example, Bob simply can't enter the train going in the direction of Alice's home.</p>
