## Description

<div><p>Vasya has gotten interested in programming contests in TCMCF+++ rules. On the contest <span class="tex-span"><i>n</i></span> problems were suggested and every problem had a cost — a certain integral number of points (perhaps, negative or even equal to zero). According to TCMCF+++ rules, only accepted problems can earn points and the overall number of points of a contestant was equal to the product of the costs of all the problems he/she had completed. If a person didn't solve anything, then he/she didn't even appear in final standings and wasn't considered as participant. Vasya understood that to get the maximal number of points it is not always useful to solve all the problems. Unfortunately, he understood it only after the contest was finished. Now he asks you to help him: find out what problems he had to solve to earn the maximal number of points.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of the suggested problems. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the cost of the <span class="tex-span"><i>i</i></span>-th task. The tasks' costs may coinсide.</p></div><div class="output-specification"><p>Print space-separated <span class="tex-font-style-bf">the costs of the problems</span> that needed to be solved to get the maximal possible number of points. Do not forget, please, that it was necessary to solve at least one problem. If there are several solutions to that problem, print any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of the suggested problems. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 100 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the cost of the <span class="tex-span"><i>i</i></span>-th task. The tasks' costs may coinсide.</p>

## Output

<p>Print space-separated <span class="tex-font-style-bf">the costs of the problems</span> that needed to be solved to get the maximal possible number of points. Do not forget, please, that it was necessary to solve at least one problem. If there are several solutions to that problem, print any of them.</p>





```input1
5
1 2 -3 3 3

```




```input2
13
100 100 100 100 100 100 100 100 100 100 100 100 100

```




```input3
4
-2 -2 -2 -2

```




```output1
3 1 2 3 

```




```output2
100 100 100 100 100 100 100 100 100 100 100 100 100 

```




```output3
-2 -2 -2 -2 

```


