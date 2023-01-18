## Description

<div><p>Limak and Radewoosh are going to compete against each other in the upcoming algorithmic contest. They are equally skilled but they won't solve problems in the same order.</p><p>There will be <span class="tex-span"><i>n</i></span> problems. The <span class="tex-span"><i>i</i></span>-th problem has initial score <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and it takes exactly <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> minutes to solve it. Problems are sorted by difficulty&nbsp;— it's guaranteed that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p><p>A constant <span class="tex-span"><i>c</i></span> is given too, representing the speed of loosing points. Then, submitting the <span class="tex-span"><i>i</i></span>-th problem at time <span class="tex-span"><i>x</i></span> (<span class="tex-span"><i>x</i></span> minutes after the start of the contest) gives <span class="tex-span"><i>max</i>(0,  <i>p</i><sub class="lower-index"><i>i</i></sub> - <i>c</i>·<i>x</i>)</span> points.</p><p>Limak is going to solve problems in order <span class="tex-span">1, 2, ..., <i>n</i></span> (sorted increasingly by <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>). Radewoosh is going to solve them in order <span class="tex-span"><i>n</i>, <i>n</i> - 1, ..., 1</span> (sorted decreasingly by <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>). Your task is to predict the outcome&nbsp;— print the name of the winner (person who gets more points at the end) or a word "<span class="tex-font-style-tt">Tie</span>" in case of a tie.</p><p>You may assume that the duration of the competition is greater or equal than the sum of all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. That means both Limak and Radewoosh will accept all <span class="tex-span"><i>n</i></span> problems.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50, 1 ≤ <i>c</i> ≤ 1000</span>)&nbsp;— the number of problems and the constant representing the speed of loosing points.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span>)&nbsp;— initial scores.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, <i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of minutes one needs to solve the <span class="tex-span"><i>i</i></span>-th problem.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">Limak</span>" (without quotes) if Limak will get more points in total. Print "<span class="tex-font-style-tt">Radewoosh</span>" (without quotes) if Radewoosh will get more points in total. Print "<span class="tex-font-style-tt">Tie</span>" (without quotes) if Limak and Radewoosh will get the same total number of points.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50, 1 ≤ <i>c</i> ≤ 1000</span>)&nbsp;— the number of problems and the constant representing the speed of loosing points.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span>)&nbsp;— initial scores.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000, <i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of minutes one needs to solve the <span class="tex-span"><i>i</i></span>-th problem.</p>

## Output

<p>Print "<span class="tex-font-style-tt">Limak</span>" (without quotes) if Limak will get more points in total. Print "<span class="tex-font-style-tt">Radewoosh</span>" (without quotes) if Radewoosh will get more points in total. Print "<span class="tex-font-style-tt">Tie</span>" (without quotes) if Limak and Radewoosh will get the same total number of points.</p>





```input1
3 2
50 85 250
10 15 25

```




```input2
3 6
50 85 250
10 15 25

```




```input3
8 1
10 20 30 40 50 60 70 80
8 10 58 63 71 72 75 76

```




```output1
Limak

```




```output2
Radewoosh

```




```output3
Tie

```



## Note

<p>In the first sample, there are <span class="tex-span">3</span> problems. Limak solves them as follows:</p><ol> <li> Limak spends <span class="tex-span">10</span> minutes on the <span class="tex-span">1</span>-st problem and he gets <span class="tex-span">50 - <i>c</i>·10 = 50 - 2·10 = 30</span> points. </li><li> Limak spends <span class="tex-span">15</span> minutes on the <span class="tex-span">2</span>-nd problem so he submits it <span class="tex-span">10 + 15 = 25</span> minutes after the start of the contest. For the <span class="tex-span">2</span>-nd problem he gets <span class="tex-span">85 - 2·25 = 35</span> points. </li><li> He spends <span class="tex-span">25</span> minutes on the <span class="tex-span">3</span>-rd problem so he submits it <span class="tex-span">10 + 15 + 25 = 50</span> minutes after the start. For this problem he gets <span class="tex-span">250 - 2·50 = 150</span> points. </li></ol><p>So, Limak got <span class="tex-span">30 + 35 + 150 = 215</span> points.</p><p>Radewoosh solves problem in the reversed order:</p><ol> <li> Radewoosh solves <span class="tex-span">3</span>-rd problem after <span class="tex-span">25</span> minutes so he gets <span class="tex-span">250 - 2·25 = 200</span> points. </li><li> He spends <span class="tex-span">15</span> minutes on the <span class="tex-span">2</span>-nd problem so he submits it <span class="tex-span">25 + 15 = 40</span> minutes after the start. He gets <span class="tex-span">85 - 2·40 = 5</span> points for this problem. </li><li> He spends <span class="tex-span">10</span> minutes on the <span class="tex-span">1</span>-st problem so he submits it <span class="tex-span">25 + 15 + 10 = 50</span> minutes after the start. He gets <span class="tex-span"><i>max</i>(0, 50 - 2·50) = <i>max</i>(0,  - 50) = 0</span> points. </li></ol><p>Radewoosh got <span class="tex-span">200 + 5 + 0 = 205</span> points in total. Limak has <span class="tex-span">215</span> points so Limak wins.</p><p>In the second sample, Limak will get <span class="tex-span">0</span> points for each problem and Radewoosh will first solve the hardest problem and he will get <span class="tex-span">250 - 6·25 = 100</span> points for that. Radewoosh will get <span class="tex-span">0</span> points for other two problems but he is the winner anyway.</p><p>In the third sample, Limak will get <span class="tex-span">2</span> points for the <span class="tex-span">1</span>-st problem and <span class="tex-span">2</span> points for the <span class="tex-span">2</span>-nd problem. Radewoosh will get <span class="tex-span">4</span> points for the <span class="tex-span">8</span>-th problem. They won't get points for other problems and thus there is a tie because <span class="tex-span">2 + 2 = 4</span>.</p>
