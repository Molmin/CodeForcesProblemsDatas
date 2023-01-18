## Description

<div><p>You have <span class="tex-span"><i>n</i></span> problems. You have estimated the difficulty of the <span class="tex-span"><i>i</i></span>-th one as integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. Now you want to prepare a problemset for a contest, using some of the problems you've made.</p><p>A problemset for the contest must consist of at least two problems. You think that the total difficulty of the problems of the contest must be at least <span class="tex-span"><i>l</i></span> and at most <span class="tex-span"><i>r</i></span>. Also, you think that the difference between difficulties of the easiest and the hardest of the chosen problems must be at least <span class="tex-span"><i>x</i></span>.</p><p>Find the number of ways to choose a problemset for the contest.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of problems you have, the minimum and maximum value of total difficulty of the problemset and the minimum difference in difficulty between the hardest problem in the pack and the easiest one, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the difficulty of each problem.</p></div><div class="output-specification"><p>Print the number of ways to choose a suitable problemset for the contest. </p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 15</span>, <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of problems you have, the minimum and maximum value of total difficulty of the problemset and the minimum difference in difficulty between the hardest problem in the pack and the easiest one, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the difficulty of each problem.</p>

## Output

<p>Print the number of ways to choose a suitable problemset for the contest. </p>





```input1
3 5 6 1
1 2 3

```




```input2
4 40 50 10
10 20 30 25

```




```input3
5 25 35 10
10 10 20 10 20

```




```output1
2

```




```output2
2

```




```output3
6

```



## Note

<p>In the first example two sets are suitable, one consisting of the second and third problem, another one consisting of all three problems.</p><p>In the second example, two sets of problems are suitable — the set of problems with difficulties 10 and 30 as well as the set of problems with difficulties 20 and 30.</p><p>In the third example any set consisting of one problem of difficulty 10 and one problem of difficulty 20 is suitable.</p>
