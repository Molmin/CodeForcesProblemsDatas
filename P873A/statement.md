## Description

<div><p>Luba has to do <span class="tex-span"><i>n</i></span> chores today. <span class="tex-span"><i>i</i></span>-th chore takes <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> units of time to complete. It is guaranteed that for every <img align="middle" class="tex-formula" src="file://U7wjxanA.png" style="max-width: 100.0%;max-height: 100.0%;"> the condition <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span> is met, so the sequence is sorted.</p><p>Also Luba can work really hard on some chores. She can choose not more than <span class="tex-span"><i>k</i></span> any chores and do each of them in <span class="tex-span"><i>x</i></span> units of time instead of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://2eQlRinI.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>Luba is very responsible, so she has to do all <span class="tex-span"><i>n</i></span> chores, and now she wants to know the minimum time she needs to do everything. Luba cannot do two chores simultaneously.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>x</i>&nbsp;(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100, 1 ≤ <i>x</i> ≤ 99</span>) — the number of chores Luba has to do, the number of chores she can do in <span class="tex-span"><i>x</i></span> units of time, and the number <span class="tex-span"><i>x</i></span> itself.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the time Luba has to spend to do <span class="tex-span"><i>i</i></span>-th chore.</p><p>It is guaranteed that <img align="middle" class="tex-formula" src="file://EAtqATMe.png" style="max-width: 100.0%;max-height: 100.0%;">, and for each <img align="middle" class="tex-formula" src="file://DoPOxuWY.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span>.</p></div><div class="output-specification"><p>Print one number — minimum time Luba needs to do all <span class="tex-span"><i>n</i></span> chores.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>x</i>&nbsp;(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100, 1 ≤ <i>x</i> ≤ 99</span>) — the number of chores Luba has to do, the number of chores she can do in <span class="tex-span"><i>x</i></span> units of time, and the number <span class="tex-span"><i>x</i></span> itself.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(2 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the time Luba has to spend to do <span class="tex-span"><i>i</i></span>-th chore.</p><p>It is guaranteed that <img align="middle" class="tex-formula" src="file://EAtqATMe.png" style="max-width: 100.0%;max-height: 100.0%;">, and for each <img align="middle" class="tex-formula" src="file://DoPOxuWY.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≥ <i>a</i><sub class="lower-index"><i>i</i> - 1</sub></span>.</p>

## Output

<p>Print one number — minimum time Luba needs to do all <span class="tex-span"><i>n</i></span> chores.</p>





```input1
4 2 2
3 6 7 10

```




```input2
5 2 1
100 100 100 100 100

```




```output1
13

```




```output2
302

```



## Note

<p>In the first example the best option would be to do the third and the fourth chore, spending <span class="tex-span"><i>x</i> = 2</span> time on each instead of <span class="tex-span"><i>a</i><sub class="lower-index">3</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">4</sub></span>, respectively. Then the answer is <span class="tex-span">3 + 6 + 2 + 2 = 13</span>.</p><p>In the second example Luba can choose any two chores to spend <span class="tex-span"><i>x</i></span> time on them instead of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. So the answer is <span class="tex-span">100·3 + 2·1 = 302</span>.</p>
