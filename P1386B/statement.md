## Description

<div><p>Serge, the chef of the famous restaurant "Salt, Pepper &amp; Garlic" is trying to obtain his first Michelin star. He has been informed that a secret expert plans to visit his restaurant this evening.</p><p>Even though the expert's name hasn't been disclosed, Serge is certain he knows which dish from the menu will be ordered as well as what the taste preferences of the expert are. Namely, the expert requires an extremely precise proportion of salt, pepper and garlic powder in his dish.</p><p>Serge keeps a set of bottles with mixtures of salt, pepper and garlic powder on a special shelf in the kitchen. For each bottle, he knows the exact amount of each of the ingredients in kilograms. Serge can combine any number of bottled mixtures (or just use one of them directly) to get a mixture of particular proportions needed for a certain dish.</p><p>Luckily, the absolute amount of a mixture that needs to be added to a dish is so small that you can assume that the amounts in the bottles will always be sufficient. However, the numeric values describing the proportions may be quite large.</p><p>Serge would like to know whether it is possible to obtain the expert's favourite mixture from the available bottles, and if so—what is the smallest possible number of bottles needed to achieve that.</p><p>Furthermore, the set of bottles on the shelf may change over time as Serge receives new ones or lends his to other chefs. So he would like to answer this question after each such change.</p><p>For example, assume that expert's favorite mixture is $1:1:1$ and there are three bottles of mixtures on the shelf:</p><center> $$ \begin{array}{cccc} \hline \text{Mixture} &amp; \text{Salt} &amp; \text{Pepper} &amp; \text{Garlic powder} \\ \hline 1 &amp; 10 &amp; 20 &amp; 30 \\ 2 &amp; 300 &amp; 200 &amp; 100 \\ 3 &amp; 12 &amp; 15 &amp; 27 \\ \hline \end{array} $$ Amount of ingredient in the bottle, kg </center><p>To obtain the desired mixture it is enough to use an equivalent amount of mixtures from bottles 1 and 2. If bottle 2 is removed, then it is no longer possible to obtain it.</p><p>Write a program that helps Serge to solve this task!</p></div><div class="input-specification"><p>The first row contains three non-negative integers $S_f$, $P_f$ and $G_f$ ($0 \leq S_f, P_f, G_f$; $0 &lt; S_f+P_f+G_f \leq 10^6$) describing the amount of salt, pepper and garlic powder in the expert's favourite mixture. For any real $\alpha&gt;0$, $(\alpha{S_f}, \alpha{P_f}, \alpha{G_f})$ also is an expert's favourite mixture.</p><p>In the second row, there is a positive integer $N$ (number of changes on the shelf, $N \leq 100\,000$). You should assume that initially the shelf is empty.</p><p>Each of the next $N$ rows describes a single change on the shelf: </p><ul> <li> If a new bottle is added, the row contains capital letter $A$ followed by three non-negative integers $S_i$, $P_i$ and $G_i$ ($0 \leq S_i, P_i, G_i$; $0 &lt; S_i+P_i+G_i \leq 10^6$) describing the amount of salt, pepper and garlic powder in the added bottle. Added bottles are numbered consecutively by unique integers starting from $1$, that is, the $i$-th bottle corresponds to the $i$-th added bottle in the input data. </li><li> If a particular bottle is removed from the shelf, the row contains capital letter $R$ followed by the integer—the bottle number $r_i$. All values $r_i$ in the removals are unique, $r_i$ never exceeds total number of bottles added thus far. </li></ul></div><div class="output-specification"><p>Output $N$ rows. The $j$-th row ($1 \leq j \leq N$) should contain the number $x_j$, the smallest number of bottles needed to prepare a mixture with the expert's favourite proportions of salt, pepper and garlic powder using the bottles available after the first $j$ changes on the shelf, or $0$ if it is not possible.</p></div><div><h2>Scoring</h2><p>Subtasks: </p><ol> <li> (13 points) $N \leq 50$, $0 &lt; S_i+P_i+G_i \leq 10^2$ </li><li> (17 points) $N \leq 500$, $0 &lt; S_i+P_i+G_i \leq 10^3$ </li><li> (30 points) $N \leq 5000$, $0 &lt; S_i+P_i+G_i \leq 10^4$ </li><li> (40 points) No further constraints </li></ol></div>

## Input

<p>The first row contains three non-negative integers $S_f$, $P_f$ and $G_f$ ($0 \leq S_f, P_f, G_f$; $0 &lt; S_f+P_f+G_f \leq 10^6$) describing the amount of salt, pepper and garlic powder in the expert's favourite mixture. For any real $\alpha&gt;0$, $(\alpha{S_f}, \alpha{P_f}, \alpha{G_f})$ also is an expert's favourite mixture.</p><p>In the second row, there is a positive integer $N$ (number of changes on the shelf, $N \leq 100\,000$). You should assume that initially the shelf is empty.</p><p>Each of the next $N$ rows describes a single change on the shelf: </p><ul> <li> If a new bottle is added, the row contains capital letter $A$ followed by three non-negative integers $S_i$, $P_i$ and $G_i$ ($0 \leq S_i, P_i, G_i$; $0 &lt; S_i+P_i+G_i \leq 10^6$) describing the amount of salt, pepper and garlic powder in the added bottle. Added bottles are numbered consecutively by unique integers starting from $1$, that is, the $i$-th bottle corresponds to the $i$-th added bottle in the input data. </li><li> If a particular bottle is removed from the shelf, the row contains capital letter $R$ followed by the integer—the bottle number $r_i$. All values $r_i$ in the removals are unique, $r_i$ never exceeds total number of bottles added thus far. </li></ul>

## Output

<p>Output $N$ rows. The $j$-th row ($1 \leq j \leq N$) should contain the number $x_j$, the smallest number of bottles needed to prepare a mixture with the expert's favourite proportions of salt, pepper and garlic powder using the bottles available after the first $j$ changes on the shelf, or $0$ if it is not possible.</p>





```input1
1 2 3
6
A 5 6 7
A 3 10 17
R 1
A 15 18 21
A 5 10 15
R 3
```




```output1
0
2
0
2
1
1
```



## Note

<p>Pay attention that in the example, bottles $1$ and $3$ contain the same proportions of salt, pepper and garlic powder.</p>
