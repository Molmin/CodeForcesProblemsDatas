## Description

<div><p><span class="tex-font-style-it">This is the easy version of the problem. The only difference between easy and hard versions is the constraint of $m$. You can make hacks only if both versions are solved.</span></p><p>Chiori loves dolls and now she is going to decorate her bedroom!</p><center><img class="tex-graphics" src="file://bVwT5hlP.png" style="max-width: 100.0%;max-height: 100.0%;"></center>&nbsp;<p>As a doll collector, Chiori has got $n$ dolls. The $i$-th doll has a non-negative integer value $a_i$ ($a_i &lt; 2^m$, $m$ is given). Chiori wants to pick some (maybe zero) dolls for the decoration, so there are $2^n$ different picking ways.</p><p>Let $x$ be the bitwise-xor-sum of values of dolls Chiori picks (in case Chiori picks no dolls $x = 0$). The value of this picking way is equal to the number of $1$-bits in the binary representation of $x$. More formally, it is also equal to the number of indices $0 \leq i &lt; m$, such that $\left\lfloor \frac{x}{2^i} \right\rfloor$ is odd.</p><p>Tell her the number of picking ways with value $i$ for each integer $i$ from $0$ to $m$. Due to the answers can be very huge, print them by modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $0 \le m \le 35$) &nbsp;— the number of dolls and the maximum value of the picking way.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^m$) &nbsp;— the values of dolls.</p></div><div class="output-specification"><p>Print $m+1$ integers $p_0, p_1, \ldots, p_m$ &nbsp;— $p_i$ is equal to the number of picking ways with value $i$ by modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $0 \le m \le 35$) &nbsp;— the number of dolls and the maximum value of the picking way.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i &lt; 2^m$) &nbsp;— the values of dolls.</p>

## Output

<p>Print $m+1$ integers $p_0, p_1, \ldots, p_m$ &nbsp;— $p_i$ is equal to the number of picking ways with value $i$ by modulo $998\,244\,353$.</p>





```input1
4 4
3 5 8 14
```




```input2
6 7
11 45 14 9 19 81
```




```output1
2 2 6 6 0
```




```output2
1 2 11 20 15 10 5 0
```


