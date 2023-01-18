## Description

<div><p>At the beginning of the new semester there is new schedule in the Berland State University. According to this schedule, <span class="tex-span"><i>n</i></span> groups have lessons at the room 31. For each group the starting time of the lesson and the finishing time of the lesson are known. It has turned out that it is impossible to hold all lessons, because for some groups periods of their lessons intersect. If at some moment of time one groups finishes it's lesson, and the other group starts the lesson, their lessons don't intersect.</p><p>The dean wants to cancel the lesson in one group so that no two time periods of lessons of the remaining groups intersect. You are to find all ways to do that.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — amount of groups, which have lessons in the room 31. Then <span class="tex-span"><i>n</i></span> lines follow, each of them contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — starting and finishing times of lesson of the <span class="tex-span"><i>i</i></span>-th group. It is possible that initially no two lessons intersect (see sample 1).</p></div><div class="output-specification"><p>Output integer <span class="tex-span"><i>k</i></span> — amount of ways to cancel the lesson in exactly one group so that no two time periods of lessons of the remaining groups intersect. In the second line output <span class="tex-span"><i>k</i></span> numbers — indexes of groups, where it is possible to cancel the lesson. Groups are numbered starting from <span class="tex-span">1</span> in the order that they were given in the input. Output the numbers in increasing order.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — amount of groups, which have lessons in the room 31. Then <span class="tex-span"><i>n</i></span> lines follow, each of them contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — starting and finishing times of lesson of the <span class="tex-span"><i>i</i></span>-th group. It is possible that initially no two lessons intersect (see sample 1).</p>

## Output

<p>Output integer <span class="tex-span"><i>k</i></span> — amount of ways to cancel the lesson in exactly one group so that no two time periods of lessons of the remaining groups intersect. In the second line output <span class="tex-span"><i>k</i></span> numbers — indexes of groups, where it is possible to cancel the lesson. Groups are numbered starting from <span class="tex-span">1</span> in the order that they were given in the input. Output the numbers in increasing order.</p>





```input1
3
3 10
20 30
1 3

```




```input2
4
3 10
20 30
1 3
1 39

```




```input3
3
1 5
2 6
3 7

```




```output1
3
1 2 3
```




```output2
1
4
```




```output3
0

```


