## Description

<div><p>Berland Football Cup starts really soon! Commentators from all over the world come to the event.</p><p>Organizers have already built $n$ commentary boxes. $m$ regional delegations will come to the Cup. Every delegation should get the <span class="tex-font-style-it">same number</span> of the commentary boxes. If any box is left unoccupied then the delegations will be upset. <span class="tex-font-style-it">So each box should be occupied by exactly one delegation.</span></p><p>If $n$ is not divisible by $m$, it is impossible to distribute the boxes to the delegations at the moment.</p><p>Organizers can build a new commentary box paying $a$ burles and demolish a commentary box paying $b$ burles. They can both build and demolish boxes arbitrary number of times (each time paying a corresponding fee). It is allowed to demolish all the existing boxes.</p><p>What is the minimal amount of burles organizers should pay to satisfy all the delegations (i.e. to make the number of the boxes be divisible by $m$)?</p></div><div class="input-specification"><p>The only line contains four integer numbers $n$, $m$, $a$ and $b$ ($1 \le n, m \le 10^{12}$, $1 \le a, b \le 100$), where $n$ is the initial number of the commentary boxes, $m$ is the number of delegations to come, $a$ is the fee to build a box and $b$ is the fee to demolish a box.</p></div><div class="output-specification"><p>Output the minimal amount of burles organizers should pay to satisfy all the delegations (i.e. to make the number of the boxes be divisible by $m$). It is allowed that the final number of the boxes is equal to $0$.</p></div>

## Input

<p>The only line contains four integer numbers $n$, $m$, $a$ and $b$ ($1 \le n, m \le 10^{12}$, $1 \le a, b \le 100$), where $n$ is the initial number of the commentary boxes, $m$ is the number of delegations to come, $a$ is the fee to build a box and $b$ is the fee to demolish a box.</p>

## Output

<p>Output the minimal amount of burles organizers should pay to satisfy all the delegations (i.e. to make the number of the boxes be divisible by $m$). It is allowed that the final number of the boxes is equal to $0$.</p>





```input1
9 7 3 8

```




```input2
2 7 3 7

```




```input3
30 6 17 19

```




```output1
15

```




```output2
14

```




```output3
0

```



## Note

<p>In the first example organizers can build $5$ boxes to make the total of $14$ paying $3$ burles for the each of them.</p><p>In the second example organizers can demolish $2$ boxes to make the total of $0$ paying $7$ burles for the each of them.</p><p>In the third example organizers are already able to distribute all the boxes equally among the delegations, each one get $5$ boxes.</p>
