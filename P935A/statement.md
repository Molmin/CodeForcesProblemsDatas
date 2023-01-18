## Description

<div><p>Fafa owns a company that works on huge projects. There are <span class="tex-span"><i>n</i></span> employees in Fafa's company. Whenever the company has a new project to start working on, Fafa has to divide the tasks of this project among all the employees.</p><p>Fafa finds doing this every time is very tiring for him. So, he decided to choose the best <span class="tex-span"><i>l</i></span> employees in his company as team leaders. Whenever there is a new project, Fafa will divide the tasks among only the team leaders and each team leader will be responsible of some positive number of employees to give them the tasks. To make this process fair for the team leaders, each one of them should be responsible for the same number of employees. Moreover, every employee, who is not a team leader, has to be under the responsibility of exactly one team leader, and no team leader is responsible for another team leader.</p><p>Given the number of employees <span class="tex-span"><i>n</i></span>, find in how many ways Fafa could choose the number of team leaders <span class="tex-span"><i>l</i></span> in such a way that it is possible to divide employees between them evenly.</p></div><div class="input-specification"><p>The input consists of a single line containing a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of employees in Fafa's company.</p></div><div class="output-specification"><p>Print a single integer representing the answer to the problem.</p></div>

## Input

<p>The input consists of a single line containing a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of employees in Fafa's company.</p>

## Output

<p>Print a single integer representing the answer to the problem.</p>





```input1
2

```




```input2
10

```




```output1
1

```




```output2
3

```



## Note

<p>In the second sample Fafa has 3 ways:</p><ul> <li> choose only <span class="tex-span">1</span> employee as a team leader with <span class="tex-span">9</span> employees under his responsibility. </li><li> choose <span class="tex-span">2</span> employees as team leaders with <span class="tex-span">4</span> employees under the responsibility of each of them. </li><li> choose <span class="tex-span">5</span> employees as team leaders with <span class="tex-span">1</span> employee under the responsibility of each of them. </li></ul>
