## Description

<div><p>Makes solves problems on Decoforces and lots of other different online judges. Each problem is denoted by its difficulty — a positive integer number. Difficulties are measured the same across all the judges (the problem with difficulty <span class="tex-span"><i>d</i></span> on Decoforces is as hard as the problem with difficulty <span class="tex-span"><i>d</i></span> on any other judge). </p><p>Makes has chosen <span class="tex-span"><i>n</i></span> problems to solve on Decoforces with difficulties <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. He can solve these problems in arbitrary order. Though he can solve problem <span class="tex-span"><i>i</i></span> with difficulty <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> only if he had already solved some problem with difficulty <img align="middle" class="tex-formula" src="file://R4ZUibPS.png" style="max-width: 100.0%;max-height: 100.0%;"> (no matter on what online judge was it).</p><p><span class="tex-font-style-it">Before starting this chosen list of problems, Makes has already solved problems with maximum difficulty <span class="tex-span"><i>k</i></span>.</span></p><p>With given conditions it's easy to see that Makes sometimes can't solve all the chosen problems, no matter what order he chooses. So he wants to solve some problems on other judges to finish solving problems from his list. </p><p><span class="tex-font-style-it">For every positive integer <span class="tex-span"><i>y</i></span> there exist some problem with difficulty <span class="tex-span"><i>y</i></span> on at least one judge besides Decoforces.</span></p><p>Makes can solve problems on any judge at any time, it isn't necessary to do problems from the chosen list one right after another.</p><p>Makes doesn't have too much free time, so he asked you to calculate the minimum number of problems he should solve on other judges in order to solve all the chosen problems from Decoforces.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print minimum number of problems Makes should solve on other judges in order to solve all chosen problems on Decoforces.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print minimum number of problems Makes should solve on other judges in order to solve all chosen problems on Decoforces.</p>





```input1
3 3
2 1 9

```




```input2
4 20
10 3 6 3

```




```output1
1

```




```output2
0

```



## Note

<p>In the first example Makes at first solves problems <span class="tex-font-style-tt">1</span> and <span class="tex-font-style-tt">2</span>. Then in order to solve the problem with difficulty <span class="tex-font-style-tt">9</span>, he should solve problem with difficulty no less than <span class="tex-font-style-tt">5</span>. The only available are difficulties <span class="tex-font-style-tt">5</span> and <span class="tex-font-style-tt">6</span> on some other judge. Solving any of these will give Makes opportunity to solve problem <span class="tex-font-style-tt">3</span>.</p><p>In the second example he can solve every problem right from the start.</p>
