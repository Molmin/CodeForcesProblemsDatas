## Description

<div><p>Bankopolis is an incredible city in which all the <span class="tex-span"><i>n</i></span> crossroads are located on a straight line and numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> along it. On each crossroad there is a bank office.</p><p>The crossroads are connected with <span class="tex-span"><i>m</i></span> oriented bicycle lanes (the <span class="tex-span"><i>i</i></span>-th lane goes from crossroad <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to crossroad <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>), the difficulty of each of the lanes is known.</p><p>Oleg the bank client wants to gift happiness and joy to the bank employees. He wants to visit exactly <span class="tex-span"><i>k</i></span> offices, in each of them he wants to gift presents to the employees.</p><p>The problem is that Oleg don't want to see the reaction on his gifts, so he can't use a bicycle lane which passes near the office in which he has already presented his gifts (formally, the <span class="tex-span"><i>i</i></span>-th lane passes near the office on the <span class="tex-span"><i>x</i></span>-th crossroad if and only if <span class="tex-span"><i>min</i>(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>) &lt; <i>x</i> &lt; <i>max</i>(<i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>)))</span>. Of course, in each of the offices Oleg can present gifts exactly once. Oleg is going to use exactly <span class="tex-span"><i>k</i> - 1</span> bicycle lane to move between offices. Oleg can start his path from any office and finish it in any office.</p><p>Oleg wants to choose such a path among possible ones that the total difficulty of the lanes he will use is minimum possible. Find this minimum possible total difficulty.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 80</span>)&nbsp;— the number of crossroads (and offices) and the number of offices Oleg wants to visit.</p><p>The second line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 2000</span>)&nbsp;— the number of bicycle lanes in Bankopolis.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain information about the lanes.</p><p>The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), denoting the crossroads connected by the <span class="tex-span"><i>i</i></span>-th road and its difficulty.</p></div><div class="output-specification"><p>In the only line print the minimum possible total difficulty of the lanes in a valid path, or <span class="tex-font-style-tt">-1</span> if there are no valid paths.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 80</span>)&nbsp;— the number of crossroads (and offices) and the number of offices Oleg wants to visit.</p><p>The second line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ 2000</span>)&nbsp;— the number of bicycle lanes in Bankopolis.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain information about the lanes.</p><p>The <span class="tex-span"><i>i</i></span>-th of these lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), denoting the crossroads connected by the <span class="tex-span"><i>i</i></span>-th road and its difficulty.</p>

## Output

<p>In the only line print the minimum possible total difficulty of the lanes in a valid path, or <span class="tex-font-style-tt">-1</span> if there are no valid paths.</p>





```input1
7 4
4
1 6 2
6 2 2
2 4 2
2 7 1

```




```input2
4 3
4
2 1 2
1 3 2
3 4 2
4 1 1

```




```output1
6

```




```output2
3

```



## Note

<p>In the first example Oleg visiting banks by path <span class="tex-span">1 → 6 → 2 → 4</span>.</p><p>Path <span class="tex-span">1 → 6 → 2 → 7</span> with smaller difficulity is incorrect because crossroad <span class="tex-span">2 → 7</span> passes near already visited office on the crossroad <span class="tex-span">6</span>.</p><p>In the second example Oleg can visit banks by path <span class="tex-span">4 → 1 → 3</span>.</p>
