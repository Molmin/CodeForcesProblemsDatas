## Description

<div><p>Pasha is participating in a contest on one well-known website. This time he wants to win the contest and will do anything to get to the first place!</p><p>This contest consists of <span class="tex-span"><i>n</i></span> problems, and Pasha solves <span class="tex-span"><i>i</i></span>th problem in <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> time units (his solutions are always correct). At any moment of time he can be thinking about a solution to only one of the problems (that is, he cannot be solving two problems at the same time). The time Pasha spends to send his solutions is negligible. <span class="tex-font-style-bf">Pasha can send any number of solutions at the same moment.</span></p><p>Unfortunately, there are too many participants, and the website is not always working. Pasha received the information that the website will be working only during <span class="tex-span"><i>m</i></span> time periods, <span class="tex-span"><i>j</i></span>th period is represented by its starting moment <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and ending moment <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>. Of course, Pasha can send his solution only when the website is working. In other words, Pasha can send his solution at some moment <span class="tex-span"><i>T</i></span> iff there exists a period <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>l</i><sub class="lower-index"><i>x</i></sub> ≤ <i>T</i> ≤ <i>r</i><sub class="lower-index"><i>x</i></sub></span>.</p><p>Pasha wants to know his best possible result. We need to tell him the minimal moment of time by which he is able to have <span class="tex-font-style-bf">solutions to all problems submitted</span>, if he acts optimally, or say that it's impossible no matter how Pasha solves the problems.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 1000)</span> — the number of problems. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the time Pasha needs to solve <span class="tex-span"><i>i</i></span>th problem.</p><p>The third line contains one integer <span class="tex-span"><i>m</i>&nbsp;(0 ≤ <i>m</i> ≤ 1000)</span> — the number of periods of time when the website is working. Next <span class="tex-span"><i>m</i></span> lines represent these periods. <span class="tex-span"><i>j</i></span>th line contains two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub>&nbsp;(1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> &lt; <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the starting and the ending moment of <span class="tex-span"><i>j</i></span>th period.</p><p><span class="tex-font-style-bf">It is guaranteed that the periods are not intersecting and are given in chronological order, so for every <span class="tex-span"><i>j</i> &gt; 1</span> the condition <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> &gt; <i>r</i><sub class="lower-index"><i>j</i> - 1</sub></span> is met.</span></p></div><div class="output-specification"><p>If Pasha can solve and submit all the problems before the end of the contest, print the minimal moment of time by which he can have all the solutions submitted.</p><p>Otherwise print "-1" (without brackets).</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 1000)</span> — the number of problems. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the time Pasha needs to solve <span class="tex-span"><i>i</i></span>th problem.</p><p>The third line contains one integer <span class="tex-span"><i>m</i>&nbsp;(0 ≤ <i>m</i> ≤ 1000)</span> — the number of periods of time when the website is working. Next <span class="tex-span"><i>m</i></span> lines represent these periods. <span class="tex-span"><i>j</i></span>th line contains two numbers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub>&nbsp;(1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> &lt; <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the starting and the ending moment of <span class="tex-span"><i>j</i></span>th period.</p><p><span class="tex-font-style-bf">It is guaranteed that the periods are not intersecting and are given in chronological order, so for every <span class="tex-span"><i>j</i> &gt; 1</span> the condition <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub> &gt; <i>r</i><sub class="lower-index"><i>j</i> - 1</sub></span> is met.</span></p>

## Output

<p>If Pasha can solve and submit all the problems before the end of the contest, print the minimal moment of time by which he can have all the solutions submitted.</p><p>Otherwise print "-1" (without brackets).</p>





```input1
2
3 4
2
1 4
7 9

```




```input2
1
5
1
1 4

```




```input3
1
5
1
1 5

```




```output1
7

```




```output2
-1

```




```output3
5

```



## Note

<p>In the first example Pasha can act like this: he solves the second problem in 4 units of time and sends it immediately. Then he spends 3 time units to solve the first problem and sends it 7 time units after the contest starts, because at this moment the website starts working again.</p><p>In the second example Pasha invents the solution only after the website stops working for the last time.</p><p>In the third example Pasha sends the solution exactly at the end of the first period.</p>
