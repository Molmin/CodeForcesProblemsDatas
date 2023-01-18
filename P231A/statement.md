## Description

<div><p>One day three best friends Petya, Vasya and Tonya decided to form a team and take part in programming contests. Participants are usually offered several problems during programming contests. Long before the start the friends decided that they will implement a problem if at least two of them are sure about the solution. Otherwise, the friends won't write the problem's solution.</p><p>This contest offers <span class="tex-span"><i>n</i></span> problems to the participants. For each problem we know, which friend is sure about the solution. Help the friends find the number of problems for which they will write a solution.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of problems in the contest. Then <span class="tex-span"><i>n</i></span> lines contain three integers each, each integer is either <span class="tex-span">0</span> or <span class="tex-span">1</span>. If the first number in the line equals <span class="tex-span">1</span>, then Petya is sure about the problem's solution, otherwise he isn't sure. The second number shows Vasya's view on the solution, the third number shows Tonya's view. The numbers on the lines are separated by spaces.</p></div><div class="output-specification"><p>Print a single integer — the number of problems the friends will implement on the contest.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of problems in the contest. Then <span class="tex-span"><i>n</i></span> lines contain three integers each, each integer is either <span class="tex-span">0</span> or <span class="tex-span">1</span>. If the first number in the line equals <span class="tex-span">1</span>, then Petya is sure about the problem's solution, otherwise he isn't sure. The second number shows Vasya's view on the solution, the third number shows Tonya's view. The numbers on the lines are separated by spaces.</p>

## Output

<p>Print a single integer — the number of problems the friends will implement on the contest.</p>





```input1
3
1 1 0
1 1 1
1 0 0

```




```input2
2
1 0 0
0 1 1

```




```output1
2

```




```output2
1

```



## Note

<p>In the first sample Petya and Vasya are sure that they know how to solve the first problem and all three of them know how to solve the second problem. That means that they will write solutions for these problems. Only Petya is sure about the solution for the third problem, but that isn't enough, so the friends won't take it. </p><p>In the second sample the friends will only implement the second problem, as Vasya and Tonya are sure about the solution.</p>
