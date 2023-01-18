## Description

<div><p>Polycarp is playing a game called "Running Over The Bridges". In this game he has to run over <span class="tex-span"><i>n</i></span> bridges from the left to the right. Bridges are arranged one after the other, so the <span class="tex-span"><i>i</i></span>-th bridge begins where the <span class="tex-span">(<i>i</i> - 1)</span>-th bridge ends.</p><p>You have the following data about bridges: <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the length of the <span class="tex-span"><i>i</i></span>-th bridge and the maximum allowed time which Polycarp can spend running over the <span class="tex-span"><i>i</i></span>-th bridge. Thus, if Polycarp is in the beginning of the bridge <span class="tex-span"><i>i</i></span> at the time <span class="tex-span"><i>T</i></span> then he has to leave it at the time <span class="tex-span"><i>T</i> + <i>t</i><sub class="lower-index"><i>i</i></sub></span> or earlier. It is allowed to reach the right end of a bridge exactly at the time <span class="tex-span"><i>T</i> + <i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Polycarp can run from the left side to the right one with speed <span class="tex-span">0.5</span>, so he will run over a bridge with length <span class="tex-span"><i>s</i></span> in time <span class="tex-span">2·<i>s</i></span>. Besides, he has several magical drinks. If he uses one drink, his speed increases twice (i.e. to value 1) for <span class="tex-span"><i>r</i></span> seconds. All magical drinks are identical. Please note that Polycarp can use a drink only at <span class="tex-font-style-bf">integer</span> moments of time, and he drinks it instantly and completely. Additionally, if Polycarp uses a drink at the moment <span class="tex-span"><i>T</i></span> he can use the next drink not earlier than at the moment <span class="tex-span"><i>T</i> + <i>r</i></span>.</p><p>What is the minimal number of drinks Polycarp has to use to run over all <span class="tex-span"><i>n</i></span> bridges? If this number is not greater than <span class="tex-span">10<sup class="upper-index">5</sup></span>, then you have to find out the moments of time when Polycarp has to use each magical drink.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">12</sup></span>) — the number of bridges and the duration of the effect of a magical drink.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is equal to the length of the <span class="tex-span"><i>i</i></span>-th bridge.</p><p>The third line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is equal to the maximum allowed time which Polycarp can spend running over the <span class="tex-span"><i>i</i></span>-th bridge.</p></div><div class="output-specification"><p>The first line of the output should contain <span class="tex-span"><i>k</i></span> — the minimal number of drinks which Polycarp has to use, or <span class="tex-font-style-tt">-1</span> if there is no solution.</p><p>If the solution exists and the value of <span class="tex-span"><i>k</i></span> is not greater than <span class="tex-span">10<sup class="upper-index">5</sup></span> then output <span class="tex-span"><i>k</i></span> integers on the next line — moments of time from beginning of the game when Polycarp has to use drinks. Print the moments of time in chronological order. If there are several solutions, you can output any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>r</i> ≤ 10<sup class="upper-index">12</sup></span>) — the number of bridges and the duration of the effect of a magical drink.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>l</i><sub class="lower-index">1</sub>, <i>l</i><sub class="lower-index">2</sub>, ..., <i>l</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">6</sup></span>), where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is equal to the length of the <span class="tex-span"><i>i</i></span>-th bridge.</p><p>The third line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is equal to the maximum allowed time which Polycarp can spend running over the <span class="tex-span"><i>i</i></span>-th bridge.</p>

## Output

<p>The first line of the output should contain <span class="tex-span"><i>k</i></span> — the minimal number of drinks which Polycarp has to use, or <span class="tex-font-style-tt">-1</span> if there is no solution.</p><p>If the solution exists and the value of <span class="tex-span"><i>k</i></span> is not greater than <span class="tex-span">10<sup class="upper-index">5</sup></span> then output <span class="tex-span"><i>k</i></span> integers on the next line — moments of time from beginning of the game when Polycarp has to use drinks. Print the moments of time in chronological order. If there are several solutions, you can output any of them.</p>





```input1
1 3
7
10

```




```input2
3 3
3 3 3
3 3 2

```




```input3
3 100000
5 5 5
5 7 8

```




```input4
4 1000
1 2 3 4
10 9 10 9

```




```output1
2
0 3

```




```output2
-1

```




```output3
1
0 

```




```output4
0


```



## Note

<p>In the first case, there is only one bridge and it is clear that Polycarp cannot run over it without magical drinks. So, if he will use one magical drink on start (moment of time <span class="tex-span">0</span>), and the second one — three seconds later (moment of time <span class="tex-span">3</span>), he will be able to reach the end of the bridge in time. Please note, in this case there are several possible answers to the problem. For example, Polycarp can use the first drink at the moment of time <span class="tex-span">4</span> and the second one — at the moment of time <span class="tex-span">7</span>.</p><p>In the second case, Polycarp cannot run over all bridges even if he will use magical drinks. So, answer in this case is <span class="tex-font-style-tt">-1</span>.</p><p>In the fourth case, Polycarp can run over all bridges without magical drinks. </p>
