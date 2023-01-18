## Description

<div><p>Ivar the Boneless is a great leader. He is trying to capture Kattegat from Lagertha. The war has begun and wave after wave Ivar's warriors are falling in battle.</p><p>Ivar has $n$ warriors, he places them on a straight line in front of the main gate, in a way that the $i$-th warrior stands right after $(i-1)$-th warrior. The first warrior leads the attack.</p><p>Each attacker can take up to $a_i$ arrows before he falls to the ground, where $a_i$ is the $i$-th warrior's strength.</p><p>Lagertha orders her warriors to shoot $k_i$ arrows during the $i$-th minute, the arrows one by one hit the first still standing warrior. After all Ivar's warriors fall and all the currently flying arrows fly by, Thor smashes his hammer and all Ivar's warriors get their previous strengths back and stand up to fight again. In other words, if all warriors die in minute $t$, they will all be standing to fight at the end of minute $t$.</p><p>The battle will last for $q$ minutes, after each minute you should tell Ivar what is the number of his standing warriors.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \leq 200\,000$)&nbsp;— the number of warriors and the number of minutes in the battle.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) that represent the warriors' strengths.</p><p>The third line contains $q$ integers $k_1, k_2, \ldots, k_q$ ($1 \leq k_i \leq 10^{14}$), the $i$-th of them represents Lagertha's order at the $i$-th minute: $k_i$ arrows will attack the warriors.</p></div><div class="output-specification"><p>Output $q$ lines, the $i$-th of them is the number of standing warriors after the $i$-th minute.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \leq 200\,000$)&nbsp;— the number of warriors and the number of minutes in the battle.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \leq a_i \leq 10^9$) that represent the warriors' strengths.</p><p>The third line contains $q$ integers $k_1, k_2, \ldots, k_q$ ($1 \leq k_i \leq 10^{14}$), the $i$-th of them represents Lagertha's order at the $i$-th minute: $k_i$ arrows will attack the warriors.</p>

## Output

<p>Output $q$ lines, the $i$-th of them is the number of standing warriors after the $i$-th minute.</p>





```input1
5 5
1 2 1 2 1
3 10 1 1 1

```




```input2
4 4
1 2 3 4
9 1 10 6

```




```output1
3
5
4
4
3

```




```output2
1
4
4
1

```



## Note

<p>In the first example: </p><ul> <li> after the 1-st minute, the 1-st and 2-nd warriors die. </li><li> after the 2-nd minute all warriors die (and all arrows left over are wasted), then they will be revived thus answer is 5&nbsp;— all warriors are alive. </li><li> after the 3-rd minute, the 1-st warrior dies. </li><li> after the 4-th minute, the 2-nd warrior takes a hit and his strength decreases by 1. </li><li> after the 5-th minute, the 2-nd warrior dies. </li></ul>
