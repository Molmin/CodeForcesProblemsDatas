## Description

<div><p><span class="tex-font-style-it">This problem consists of three subproblems: for solving subproblem C1 you will receive 4 points, for solving subproblem C2 you will receive 4 points, and for solving subproblem C3 you will receive 8 points.</span></p><p>Manao decided to pursue a fighter's career. He decided to begin with an ongoing tournament. Before Manao joined, there were <span class="tex-span"><i>n</i></span> contestants in the tournament, numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each of them had already obtained some amount of tournament points, namely the <span class="tex-span"><i>i</i></span>-th fighter had <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> points.</p><p>Manao is going to engage in a single fight against each contestant. Each of Manao's fights ends in either a win or a loss. A win grants Manao one point, and a loss grants Manao's opponent one point. For each <span class="tex-span"><i>i</i></span>, Manao estimated the amount of effort <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> he needs to invest to win against the <span class="tex-span"><i>i</i></span>-th contestant. Losing a fight costs no effort.</p><p>After Manao finishes all of his fights, the ranklist will be determined, with <span class="tex-span">1</span> being the best rank and <span class="tex-span"><i>n</i> + 1</span> being the worst. The contestants will be ranked in descending order of their tournament points. The contestants with the same number of points as Manao will be ranked better than him if they won the match against him and worse otherwise. The exact mechanism of breaking ties for other fighters is not relevant here.</p><p>Manao's objective is to have rank <span class="tex-span"><i>k</i></span> or better. Determine the minimum total amount of effort he needs to invest in order to fulfill this goal, if it is possible.</p></div><div class="input-specification"><p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> + 1</span>). The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers separated by a single space — <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>).</p><p><span class="tex-font-style-it">The problem consists of three subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem C1 (4 points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 15</span> will hold. </li><li> In subproblem C2 (4 points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span> will hold. </li><li> In subproblem C3 (8 points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span> will hold. </li></ul></div><div class="output-specification"><p>Print a single number in a single line — the minimum amount of effort Manao needs to use to rank in the top <span class="tex-span"><i>k</i></span>. If no amount of effort can earn Manao such a rank, output number -1.</p></div>

## Input

<p>The first line contains a pair of integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> + 1</span>). The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers separated by a single space — <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub>, <i>e</i><sub class="lower-index"><i>i</i></sub> ≤ 200000</span>).</p><p><span class="tex-font-style-it">The problem consists of three subproblems. The subproblems have different constraints on the input. You will get some score for the correct submission of the subproblem. The description of the subproblems follows.</span></p><ul> <li> In subproblem C1 (4 points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 15</span> will hold. </li><li> In subproblem C2 (4 points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 100</span> will hold. </li><li> In subproblem C3 (8 points), the constraint <span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span> will hold. </li></ul>

## Output

<p>Print a single number in a single line — the minimum amount of effort Manao needs to use to rank in the top <span class="tex-span"><i>k</i></span>. If no amount of effort can earn Manao such a rank, output number -1.</p>





```input1
3 2
1 1
1 4
2 2

```




```input2
2 1
3 2
4 0

```




```input3
5 2
2 10
2 10
1 1
3 1
3 1

```




```output1
3

```




```output2
-1

```




```output3
12

```



## Note

<p>Consider the first test case. At the time when Manao joins the tournament, there are three fighters. The first of them has 1 tournament point and the victory against him requires 1 unit of effort. The second contestant also has 1 tournament point, but Manao needs 4 units of effort to defeat him. The third contestant has 2 points and victory against him costs Manao 2 units of effort. Manao's goal is top be in top 2. The optimal decision is to win against fighters <span class="tex-span">1</span> and <span class="tex-span">3</span>, after which Manao, fighter <span class="tex-span">2</span>, and fighter <span class="tex-span">3</span> will all have 2 points. Manao will rank better than fighter <span class="tex-span">3</span> and worse than fighter <span class="tex-span">2</span>, thus finishing in second place.</p><p>Consider the second test case. Even if Manao wins against both opponents, he will still rank third.</p>
