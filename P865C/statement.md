## Description

<div><p>You're trying to set the record on your favorite video game. The game consists of <span class="tex-span"><i>N</i></span> levels, which must be completed sequentially in order to beat the game. You usually complete each level as fast as possible, but sometimes finish a level slower. Specifically, you will complete the <span class="tex-span"><i>i</i></span>-th level in either <span class="tex-span"><i>F</i><sub class="lower-index"><i>i</i></sub></span> seconds or <span class="tex-span"><i>S</i><sub class="lower-index"><i>i</i></sub></span> seconds, where <span class="tex-span"><i>F</i><sub class="lower-index"><i>i</i></sub> &lt; <i>S</i><sub class="lower-index"><i>i</i></sub></span>, and there's a <span class="tex-span"><i>P</i><sub class="lower-index"><i>i</i></sub></span> percent chance of completing it in <span class="tex-span"><i>F</i><sub class="lower-index"><i>i</i></sub></span> seconds. After completing a level, you may decide to either continue the game and play the next level, or reset the game and start again from the first level. Both the decision and the action are instant.</p><p>Your goal is to complete all the levels sequentially in at most <span class="tex-span"><i>R</i></span> total seconds. You want to minimize the expected amount of time playing before achieving that goal. If you continue and reset optimally, how much total time can you expect to spend playing?</p></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>R</i></span> <img align="middle" class="tex-formula" src="file://PxdBlut8.png" style="max-width: 100.0%;max-height: 100.0%;">, the number of levels and number of seconds you want to complete the game in, respectively. <span class="tex-span"><i>N</i></span> lines follow. The <span class="tex-span"><i>i</i></span>th such line contains integers <span class="tex-span"><i>F</i><sub class="lower-index"><i>i</i></sub>, <i>S</i><sub class="lower-index"><i>i</i></sub>, <i>P</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>F</i><sub class="lower-index"><i>i</i></sub> &lt; <i>S</i><sub class="lower-index"><i>i</i></sub> ≤ 100, 80 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> ≤ 99)</span>, the fast time for level <span class="tex-span"><i>i</i></span>, the slow time for level <span class="tex-span"><i>i</i></span>, and the probability (as a percentage) of completing level <span class="tex-span"><i>i</i></span> with the fast time.</p></div><div class="output-specification"><p>Print the total expected time. Your answer must be correct within an absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer will be considered correct, if <img align="middle" class="tex-formula" src="file://O9RrJ6xD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>R</i></span> <img align="middle" class="tex-formula" src="file://PxdBlut8.png" style="max-width: 100.0%;max-height: 100.0%;">, the number of levels and number of seconds you want to complete the game in, respectively. <span class="tex-span"><i>N</i></span> lines follow. The <span class="tex-span"><i>i</i></span>th such line contains integers <span class="tex-span"><i>F</i><sub class="lower-index"><i>i</i></sub>, <i>S</i><sub class="lower-index"><i>i</i></sub>, <i>P</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>F</i><sub class="lower-index"><i>i</i></sub> &lt; <i>S</i><sub class="lower-index"><i>i</i></sub> ≤ 100, 80 ≤ <i>P</i><sub class="lower-index"><i>i</i></sub> ≤ 99)</span>, the fast time for level <span class="tex-span"><i>i</i></span>, the slow time for level <span class="tex-span"><i>i</i></span>, and the probability (as a percentage) of completing level <span class="tex-span"><i>i</i></span> with the fast time.</p>

## Output

<p>Print the total expected time. Your answer must be correct within an absolute or relative error of <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer will be considered correct, if <img align="middle" class="tex-formula" src="file://O9RrJ6xD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
1 8
2 8 81

```




```input2
2 30
20 30 80
3 9 85

```




```input3
4 319
63 79 89
79 97 91
75 87 88
75 90 83

```




```output1
3.14

```




```output2
31.4

```




```output3
314.159265358

```



## Note

<p>In the first example, you never need to reset. There's an <span class="tex-span">81%</span> chance of completing the level in <span class="tex-span">2</span> seconds and a <span class="tex-span">19%</span> chance of needing <span class="tex-span">8</span> seconds, both of which are within the goal time. The expected time is <span class="tex-span">0.81·2 + 0.19·8 = 3.14</span>.</p><p>In the second example, you should reset after the first level if you complete it slowly. On average it will take <span class="tex-span">0.25</span> slow attempts before your first fast attempt. Then it doesn't matter whether you complete the second level fast or slow. The expected time is <span class="tex-span">0.25·30 + 20 + 0.85·3 + 0.15·9 = 31.4</span>.</p>
