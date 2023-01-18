## Description

<div><p>At the beginning of the school year Berland State University starts two city school programming groups, for beginners and for intermediate coders. The children were tested in order to sort them into groups. According to the results, each student got some score from 1 to <span class="tex-span"><i>m</i></span> points. We know that <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> schoolchildren got 1 point, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> children got 2 points, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>m</i></sub></span> children got <span class="tex-span"><i>m</i></span> points. Now you need to set the passing rate <span class="tex-span"><i>k</i></span> (integer from 1 to <span class="tex-span"><i>m</i></span>): all schoolchildren who got less than <span class="tex-span"><i>k</i></span> points go to the beginner group and those who get at strictly least <span class="tex-span"><i>k</i></span> points go to the intermediate group. We know that if the size of a group is more than <span class="tex-span"><i>y</i></span>, then the university won't find a room for them. We also know that if a group has less than <span class="tex-span"><i>x</i></span> schoolchildren, then it is too small and there's no point in having classes with it. So, you need to split all schoolchildren into two groups so that the size of each group was from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>, inclusive. </p><p>Help the university pick the passing rate in a way that meets these requirements.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>m</i></sub></span>, separated by single spaces (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The third line contains two space-separated integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ 10000</span>). At least one <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is greater than 0.</p></div><div class="output-specification"><p>If it is impossible to pick a passing rate in a way that makes the size of each resulting groups at least <span class="tex-span"><i>x</i></span> and at most <span class="tex-span"><i>y</i></span>, print 0. Otherwise, print an integer from 1 to <span class="tex-span"><i>m</i></span> — the passing rate you'd like to suggest. If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>m</i> ≤ 100</span>). The second line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>c</i><sub class="lower-index"><i>m</i></sub></span>, separated by single spaces (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). The third line contains two space-separated integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ 10000</span>). At least one <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is greater than 0.</p>

## Output

<p>If it is impossible to pick a passing rate in a way that makes the size of each resulting groups at least <span class="tex-span"><i>x</i></span> and at most <span class="tex-span"><i>y</i></span>, print 0. Otherwise, print an integer from 1 to <span class="tex-span"><i>m</i></span> — the passing rate you'd like to suggest. If there are multiple possible answers, print any of them.</p>





```input1
5
3 4 3 2 1
6 8

```




```input2
5
0 3 3 4 2
3 10

```




```input3
2
2 5
3 6

```




```output1
3

```




```output2
4

```




```output3
0

```



## Note

<p>In the first sample the beginner group has 7 students, the intermediate group has 6 of them. </p><p>In the second sample another correct answer is 3.</p>
