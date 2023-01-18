## Description

<div><p>The employees of the R1 company often spend time together: they watch football, they go camping, they solve contests. So, it's no big deal that sometimes someone pays for someone else.</p><p>Today is the day of giving out money rewards. The R1 company CEO will invite employees into his office one by one, rewarding each one for the hard work this month. The CEO knows who owes money to whom. And he also understands that if he invites person <span class="tex-span"><i>x</i></span> to his office for a reward, and then immediately invite person <span class="tex-span"><i>y</i></span>, who has lent some money to person <span class="tex-span"><i>x</i></span>, then they can meet. Of course, in such a situation, the joy of person <span class="tex-span"><i>x</i></span> from his brand new money reward will be much less. Therefore, the R1 CEO decided to invite the staff in such an order that the described situation will not happen for any pair of employees invited one after another.</p><p>However, there are a lot of employees in the company, and the CEO doesn't have a lot of time. Therefore, the task has been assigned to you. Given the debt relationships between all the employees, determine in which order they should be invited to the office of the R1 company CEO, or determine that the described order does not exist.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://gIIseIVk.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of employees in R1 and the number of debt relations. Each of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, these integers indicate that the person number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> owes money to a person a number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Assume that all the employees are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that each pair of people <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span> is mentioned in the input data at most once. In particular, the input data will not contain pairs <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>q</i></span>, <span class="tex-span"><i>p</i></span> simultaneously.</p></div><div class="output-specification"><p>Print -1 if the described order does not exist. Otherwise, print the permutation of <span class="tex-span"><i>n</i></span> distinct integers. The first number should denote the number of the person who goes to the CEO office first, the second number denote the person who goes second and so on.</p><p>If there are multiple correct orders, you are allowed to print any of them.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://gIIseIVk.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of employees in R1 and the number of debt relations. Each of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>, these integers indicate that the person number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> owes money to a person a number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Assume that all the employees are numbered from 1 to <span class="tex-span"><i>n</i></span>.</p><p>It is guaranteed that each pair of people <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span> is mentioned in the input data at most once. In particular, the input data will not contain pairs <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span> and <span class="tex-span"><i>q</i></span>, <span class="tex-span"><i>p</i></span> simultaneously.</p>

## Output

<p>Print -1 if the described order does not exist. Otherwise, print the permutation of <span class="tex-span"><i>n</i></span> distinct integers. The first number should denote the number of the person who goes to the CEO office first, the second number denote the person who goes second and so on.</p><p>If there are multiple correct orders, you are allowed to print any of them.</p>





```input1
2 1
1 2

```




```input2
3 3
1 2
2 3
3 1

```




```output1
2 1 

```




```output2
2 1 3 

```


