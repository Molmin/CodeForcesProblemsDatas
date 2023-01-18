## Description

<div><p>People like to be fit. That's why many of them are ready to wake up at dawn, go to the stadium and run. In this problem your task is to help a company design a new stadium. </p><p>The city of N has a shabby old stadium. Many people like it and every morning thousands of people come out to this stadium to run. The stadium can be represented as a circle, its length is exactly <span class="tex-span"><i>l</i></span> meters with a marked start line. However, there can't be simultaneous start in the morning, so exactly at 7, each runner goes to his favorite spot on the stadium and starts running from there. Note that not everybody runs in the same manner as everybody else. Some people run in the clockwise direction, some of them run in the counter-clockwise direction. It mostly depends on the runner's mood in the morning, so you can assume that each running direction is equiprobable for each runner in any fixed morning. </p><p>The stadium is tiny and is in need of major repair, for right now there only is one running track! You can't get too playful on a single track, that's why all runners keep the same running speed — exactly 1 meter per a time unit. Nevertheless, the runners that choose different directions bump into each other as they meet. </p><p>The company wants to design a new stadium, but they first need to know how bad the old one is. For that they need the expectation of the number of bumpings by <span class="tex-span"><i>t</i></span> time units after the running has begun. Help the company count the required expectation. Note that each runner chooses a direction equiprobably, independently from the others and then all runners start running simultaneously at 7 a.m. Assume that each runner runs for <span class="tex-span"><i>t</i></span> time units without stopping. Consider the runners to bump at a certain moment if at that moment they found themselves at the same point in the stadium. A pair of runners can bump more than once.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> &lt; <i>l</i>)</span>, here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the clockwise distance from the start line to the <span class="tex-span"><i>i</i></span>-th runner's starting position.</p></div><div class="output-specification"><p>Print a single real number — the answer to the problem with absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>l</i> ≤ 10<sup class="upper-index">9</sup>, 1 ≤ <i>t</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> &lt; <i>l</i>)</span>, here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the clockwise distance from the start line to the <span class="tex-span"><i>i</i></span>-th runner's starting position.</p>

## Output

<p>Print a single real number — the answer to the problem with absolute or relative error of at most <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2 5 1
0 2

```




```input2
3 7 3
0 1 6

```




```output1
0.2500000000

```




```output2
1.5000000000

```



## Note

<p>There are two runners in the first example. If the first runner run clockwise direction, then in 1 time unit he will be 1m away from the start line. If the second runner run counter-clockwise direction then in 1 time unit he will be also 1m away from the start line. And it is the only possible way to meet. We assume that each running direction is equiprobable, so the answer for the example is equal to <span class="tex-span">0.5·0.5 = 0.25</span>.</p>
