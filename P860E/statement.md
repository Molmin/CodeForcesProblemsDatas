## Description

<div><p>Arkady words in a large company. There are <span class="tex-span"><i>n</i></span> employees working in a system of a strict hierarchy. Namely, each employee, with an exception of the CEO, has exactly one immediate manager. The CEO is a manager (through a chain of immediate managers) of all employees.</p><p>Each employee has an integer rank. The CEO has rank equal to <span class="tex-span">1</span>, each other employee has rank equal to the rank of his immediate manager plus <span class="tex-span">1</span>.</p><p>Arkady has a good post in the company, however, he feels that he is nobody in the company's structure, and there are a lot of people who can replace him. He introduced the value of <span class="tex-font-style-it">replaceability</span>. Consider an employee <span class="tex-span"><i>a</i></span> and an employee <span class="tex-span"><i>b</i></span>, the latter being manager of <span class="tex-span"><i>a</i></span> (not necessarily immediate). Then the replaceability <span class="tex-span"><i>r</i>(<i>a</i>, <i>b</i>)</span> of <span class="tex-span"><i>a</i></span> with respect to <span class="tex-span"><i>b</i></span> is the number of subordinates (not necessarily immediate) of the manager <span class="tex-span"><i>b</i></span>, whose rank is not greater than the rank of <span class="tex-span"><i>a</i></span>. Apart from replaceability, Arkady introduced the value of <span class="tex-font-style-it">negligibility</span>. The negligibility <span class="tex-span"><i>z</i><sub class="lower-index"><i>a</i></sub></span> of employee <span class="tex-span"><i>a</i></span> equals the sum of his replaceabilities with respect to all his managers, i.e. <img align="middle" class="tex-formula" src="file://CUstX7CR.png" style="max-width: 100.0%;max-height: 100.0%;">, where the sum is taken over all his managers <span class="tex-span"><i>b</i></span>.</p><p>Arkady is interested not only in negligibility of himself, but also in negligibility of all employees in the company. Find the negligibility of each employee for Arkady.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of employees in the company.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = 0</span> if the <span class="tex-span"><i>i</i></span>-th employee is the CEO, otherwise <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> equals the id of the immediate manager of the employee with id <span class="tex-span"><i>i</i></span>. The employees are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that there is exactly one <span class="tex-span">0</span> among these values, and also that the CEO is a manager (not necessarily immediate) for all the other employees.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— the negligibilities of all employees in the order of their ids: <span class="tex-span"><i>z</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">2</sub>, ..., <i>z</i><sub class="lower-index"><i>n</i></sub></span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of employees in the company.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> = 0</span> if the <span class="tex-span"><i>i</i></span>-th employee is the CEO, otherwise <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> equals the id of the immediate manager of the employee with id <span class="tex-span"><i>i</i></span>. The employees are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. It is guaranteed that there is exactly one <span class="tex-span">0</span> among these values, and also that the CEO is a manager (not necessarily immediate) for all the other employees.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— the negligibilities of all employees in the order of their ids: <span class="tex-span"><i>z</i><sub class="lower-index">1</sub>, <i>z</i><sub class="lower-index">2</sub>, ..., <i>z</i><sub class="lower-index"><i>n</i></sub></span>.</p>





```input1
4
0 1 2 1

```




```input2
5
2 3 4 5 0

```




```input3
5
0 1 1 1 3

```




```output1
0 2 4 2 

```




```output2
10 6 3 1 0 

```




```output3
0 3 3 3 5 

```



## Note

<p>Consider the first example: </p><ul> <li> The CEO has no managers, thus <span class="tex-span"><i>z</i><sub class="lower-index">1</sub> = 0</span>. </li><li> <span class="tex-span"><i>r</i>(2, 1) = 2</span> (employees <span class="tex-span">2</span> and <span class="tex-span">4</span> suit the conditions, employee <span class="tex-span">3</span> has too large rank). Thus <span class="tex-span"><i>z</i><sub class="lower-index">2</sub> = <i>r</i>(2, 1) = 2</span>. </li><li> Similarly, <span class="tex-span"><i>z</i><sub class="lower-index">4</sub> = <i>r</i>(4, 1) = 2</span>. </li><li> <span class="tex-span"><i>r</i>(3, 2) = 1</span> (employee <span class="tex-span">3</span> is a subordinate of <span class="tex-span">2</span> and has suitable rank). <span class="tex-span"><i>r</i>(3, 1) = 3</span> (employees <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> suit the conditions). Thus <span class="tex-span"><i>z</i><sub class="lower-index">3</sub> = <i>r</i>(3, 2) + <i>r</i>(3, 1) = 4</span>. </li></ul>
