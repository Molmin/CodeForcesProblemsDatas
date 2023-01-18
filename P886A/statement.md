## Description

<div><p>In a small but very proud high school it was decided to win ACM ICPC. This goal requires to compose as many teams of three as possible, but since there were only <span class="tex-span">6</span> students who wished to participate, the decision was to build exactly two teams.</p><p>After practice competition, participant number <span class="tex-span"><i>i</i></span> got a <span class="tex-font-style-it">score</span> of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-font-style-it">Team score</span> is defined as sum of scores of its participants. High school management is interested if it's possible to build two teams with equal scores. Your task is to answer that question.</p></div><div class="input-specification"><p>The single line contains six integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index">6</sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — scores of the participants</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity), if it is possible to build teams with equal score, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each character either upper- or lowercase ("<span class="tex-font-style-tt">YeS</span>" and "<span class="tex-font-style-tt">yes</span>" are valid when the answer is "<span class="tex-font-style-tt">YES</span>").</p></div>

## Input

<p>The single line contains six integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, ..., <i>a</i><sub class="lower-index">6</sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — scores of the participants</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity), if it is possible to build teams with equal score, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each character either upper- or lowercase ("<span class="tex-font-style-tt">YeS</span>" and "<span class="tex-font-style-tt">yes</span>" are valid when the answer is "<span class="tex-font-style-tt">YES</span>").</p>





```input1
1 3 2 1 2 1

```




```input2
1 1 1 1 1 99

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample, first team can be composed of <span class="tex-span">1</span>st, <span class="tex-span">2</span>nd and <span class="tex-span">6</span>th participant, second — of <span class="tex-span">3</span>rd, <span class="tex-span">4</span>th and <span class="tex-span">5</span>th: team scores are <span class="tex-span">1 + 3 + 1 = 2 + 1 + 2 = 5</span>.</p><p>In the second sample, score of participant number <span class="tex-span">6</span> is too high: his team score will be definitely greater.</p>
