## Description

<div><p>Petya loves football very much, especially when his parents aren't home. Each morning he comes to the yard, gathers his friends and they play all day. From time to time they have a break to have some food or do some chores (for example, water the flowers).</p><p>The key in football is to divide into teams fairly before the game begins. There are <span class="tex-span"><i>n</i></span> boys playing football in the yard (including Petya), each boy's football playing skill is expressed with a non-negative characteristic <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (the larger it is, the better the boy plays). </p><p>Let's denote the number of players in the first team as <span class="tex-span"><i>x</i></span>, the number of players in the second team as <span class="tex-span"><i>y</i></span>, the individual numbers of boys who play for the first team as <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and the individual numbers of boys who play for the second team as <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. Division <span class="tex-span"><i>n</i></span> boys into two teams is considered fair if three conditions are fulfilled:</p><ul> <li> Each boy plays for exactly one team (<span class="tex-span"><i>x</i> + <i>y</i> = <i>n</i></span>). </li><li> The sizes of teams differ in no more than one (<span class="tex-span">|<i>x</i> - <i>y</i>| ≤ 1</span>). </li><li> The total football playing skills for two teams differ in no more than by the value of skill the best player in the yard has. More formally: <center class="tex-equation"><img align="middle" class="tex-formula" src="file://djKuR3qb.png" style="max-width: 100.0%;max-height: 100.0%;"></center></li></ul><p>Your task is to help guys divide into two teams fairly. It is guaranteed that a fair division into two teams always exists.</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of guys in the yard. The next line contains <span class="tex-span"><i>n</i></span> positive space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), the <span class="tex-span"><i>i</i></span>-th number represents the <span class="tex-span"><i>i</i></span>-th boy's playing skills. </p></div><div class="output-specification"><p>On the first line print an integer <span class="tex-span"><i>x</i></span> — the number of boys playing for the first team. On the second line print <span class="tex-span"><i>x</i></span> integers — the individual numbers of boys playing for the first team. On the third line print an integer <span class="tex-span"><i>y</i></span> — the number of boys playing for the second team, on the fourth line print <span class="tex-span"><i>y</i></span> integers — the individual numbers of boys playing for the second team. Don't forget that you should fulfil all three conditions: <span class="tex-span"><i>x</i> + <i>y</i> = <i>n</i></span>, <span class="tex-span">|<i>x</i> - <i>y</i>| ≤ 1</span>, and the condition that limits the total skills.</p><p>If there are multiple ways to solve the problem, print any of them.</p><p>The boys are numbered starting from one in the order in which their skills are given in the input data. You are allowed to print individual numbers of boys who belong to the same team in any order.</p></div>

## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of guys in the yard. The next line contains <span class="tex-span"><i>n</i></span> positive space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), the <span class="tex-span"><i>i</i></span>-th number represents the <span class="tex-span"><i>i</i></span>-th boy's playing skills. </p>

## Output

<p>On the first line print an integer <span class="tex-span"><i>x</i></span> — the number of boys playing for the first team. On the second line print <span class="tex-span"><i>x</i></span> integers — the individual numbers of boys playing for the first team. On the third line print an integer <span class="tex-span"><i>y</i></span> — the number of boys playing for the second team, on the fourth line print <span class="tex-span"><i>y</i></span> integers — the individual numbers of boys playing for the second team. Don't forget that you should fulfil all three conditions: <span class="tex-span"><i>x</i> + <i>y</i> = <i>n</i></span>, <span class="tex-span">|<i>x</i> - <i>y</i>| ≤ 1</span>, and the condition that limits the total skills.</p><p>If there are multiple ways to solve the problem, print any of them.</p><p>The boys are numbered starting from one in the order in which their skills are given in the input data. You are allowed to print individual numbers of boys who belong to the same team in any order.</p>





```input1
3
1 2 1

```




```input2
5
2 3 3 1 1

```




```output1
2
1 2 
1
3 

```




```output2
3
4 1 3 
2
5 2 

```



## Note

<p>Let's consider the first sample test. There we send the first and the second boy to the first team and the third boy to the second team. Let's check all three conditions of a fair division. The first limitation is fulfilled (all boys play), the second limitation on the sizes of groups (<span class="tex-span">|2 - 1| = 1 ≤ 1</span>) is fulfilled, the third limitation on the difference in skills (<span class="tex-span">(2 + 1) - (1) = 2 ≤ 2</span>) is fulfilled.</p>
