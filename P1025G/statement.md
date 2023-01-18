## Description

<div><p>There are $n$ startups. Startups can be <span class="tex-font-style-it">active</span> or <span class="tex-font-style-it">acquired</span>. If a startup is <span class="tex-font-style-it">acquired</span>, then that means it has exactly one <span class="tex-font-style-it">active</span> startup that it is following. An active startup can have arbitrarily many acquired startups that are following it. An active startup cannot follow any other startup.</p><p>The following steps happen until there is exactly one active startup. The following sequence of steps takes exactly 1 day.</p><ol> <li> Two distinct active startups $A$, $B$, are chosen uniformly at random. </li><li> A fair coin is flipped, and with equal probability, $A$ acquires $B$ or $B$ acquires $A$ (i.e. if $A$ acquires $B$, then that means $B$'s state changes from active to acquired, and its starts following $A$). </li><li> When a startup changes from active to acquired, all of its previously acquired startups become active. </li></ol><p>For example, the following scenario can happen: Let's say $A$, $B$ are active startups. $C$, $D$, $E$ are acquired startups under $A$, and $F$, $G$ are acquired startups under $B$:</p><center> <img class="tex-graphics" height="155px" src="file://0cFdzr16.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"><p><span class="tex-font-size-small">Active startups are shown in red.</span> </p></center><p>If $A$ acquires $B$, then the state will be $A$, $F$, $G$ are active startups. $C$, $D$, $E$, $B$ are acquired startups under $A$. $F$ and $G$ have no acquired startups:</p><center> <img class="tex-graphics" height="155px" src="file://3mdWLKZl.png" style="max-width: 100.0%;max-height: 100.0%;" width="333px"> </center><p>If instead, $B$ acquires $A$, then the state will be $B$, $C$, $D$, $E$ are active startups. $F$, $G$, $A$ are acquired startups under $B$. $C$, $D$, $E$ have no acquired startups:</p><center> <img class="tex-graphics" height="159px" src="file://sdMwv6Oi.png" style="max-width: 100.0%;max-height: 100.0%;" width="370px"> </center><p>You are given the initial state of the startups. For each startup, you are told if it is either acquired or active. If it is acquired, you are also given the index of the active startup that it is following.</p><p>You're now wondering, what is the expected number of days needed for this process to finish with exactly one active startup at the end.</p><p>It can be shown the expected number of days can be written as a rational number $P/Q$, where $P$ and $Q$ are co-prime integers, and $Q \not= 0 \pmod{10^9+7}$. Return the value of $P \cdot Q^{-1}$ modulo $10^9+7$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \leq n \leq 500$), the number of startups.</p><p>The next line will contain $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($a_i = -1$ or $1 \leq a_i \leq n$). If $a_i = -1$, then that means startup $i$ is active. Otherwise, if $1 \leq a_i \leq n$, then startup $i$ is acquired, and it is currently following startup $a_i$. It is guaranteed if $a_i \not= -1$, then $a_{a_i} =-1$ (that is, all startups that are being followed are active).</p></div><div class="output-specification"><p>Print a single integer, the expected number of days needed for the process to end with exactly one active startup, modulo $10^9+7$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \leq n \leq 500$), the number of startups.</p><p>The next line will contain $n$ space-separated integers $a_1, a_2, \ldots, a_n$ ($a_i = -1$ or $1 \leq a_i \leq n$). If $a_i = -1$, then that means startup $i$ is active. Otherwise, if $1 \leq a_i \leq n$, then startup $i$ is acquired, and it is currently following startup $a_i$. It is guaranteed if $a_i \not= -1$, then $a_{a_i} =-1$ (that is, all startups that are being followed are active).</p>

## Output

<p>Print a single integer, the expected number of days needed for the process to end with exactly one active startup, modulo $10^9+7$.</p>





```input1
3
-1 -1 -1

```




```input2
2
2 -1

```




```input3
40
3 3 -1 -1 4 4 -1 -1 -1 -1 -1 10 10 10 10 10 10 4 20 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 3 3 3 3 3 3 3 3

```




```output1
3

```




```output2
0

```




```output3
755808950

```



## Note

<p>In the first sample, there are three active startups labeled $1$, $2$ and $3$, and zero acquired startups. Here's an example of how one scenario can happen</p><ol> <li> Startup $1$ acquires startup $2$ (This state can be represented by the array $[-1, 1, -1]$) </li><li> Startup $3$ acquires startup $1$ (This state can be represented by the array $[3, -1, -1]$) </li><li> Startup $2$ acquires startup $3$ (This state can be represented by the array $[-1, -1, 2]$). </li><li> Startup $2$ acquires startup $1$ (This state can be represented by the array $[2, -1, 2]$). </li></ol><p>At this point, there is only one active startup, and this sequence of steps took $4$ days. It can be shown the expected number of days is $3$.</p><p>For the second sample, there is only one active startup, so we need zero days.</p><p>For the last sample, remember to take the answer modulo $10^9+7$.</p>
