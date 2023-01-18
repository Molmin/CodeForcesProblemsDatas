## Description

<div><p>Limak is a big polar bear. He prepared <span class="tex-span"><i>n</i></span> problems for an algorithmic contest. The <span class="tex-span"><i>i</i></span>-th problem has <span class="tex-font-style-bf">initial</span> score <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Also, testers said that it takes <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> minutes to solve the <span class="tex-span"><i>i</i></span>-th problem. Problems aren't necessarily sorted by difficulty and maybe harder problems have smaller initial score but it's too late to change it&nbsp;— Limak has already announced initial scores for problems. Though it's still possible to adjust the speed of losing points, denoted by <span class="tex-span"><i>c</i></span> in this statement.</p><p>Let <span class="tex-span"><i>T</i></span> denote the total number of minutes needed to solve all problems (so, <span class="tex-span"><i>T</i> = <i>t</i><sub class="lower-index">1</sub> + <i>t</i><sub class="lower-index">2</sub> + ... + <i>t</i><sub class="lower-index"><i>n</i></sub></span>). The contest will last exactly <span class="tex-span"><i>T</i></span> minutes. So it's just enough to solve all problems.</p><p>Points given for solving a problem decrease linearly. Solving the <span class="tex-span"><i>i</i></span>-th problem after <span class="tex-span"><i>x</i></span> minutes gives exactly <img align="middle" class="tex-formula" src="file://SneUCnli.png" style="max-width: 100.0%;max-height: 100.0%;"> points, where <img align="middle" class="tex-formula" src="file://qnlRJWiO.png" style="max-width: 100.0%;max-height: 100.0%;"> is some real constant that Limak must choose.</p><p>Let's assume that <span class="tex-span"><i>c</i></span> is fixed. During a contest a participant chooses some order in which he or she solves problems. There are <span class="tex-span"><i>n</i>!</span> possible orders and each of them gives some total number of points, not necessarily integer. We say that an order is <span class="tex-font-style-it">optimal</span> if it gives the maximum number of points. In other words, the total number of points given by this order is greater or equal than the number of points given by any other order. It's obvious that there is at least one optimal order. However, there may be more than one optimal order.</p><p>Limak assumes that every participant will properly estimate <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> at the very beginning and will choose some optimal order. He also assumes that testers correctly predicted time needed to solve each problem.</p><p>For two distinct problems <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>p</i><sub class="lower-index"><i>j</i></sub></span> Limak wouldn't be happy to see a participant with strictly more points for problem <span class="tex-span"><i>i</i></span> than for problem <span class="tex-span"><i>j</i></span>. He calls such a situation a <span class="tex-font-style-it">paradox</span>.</p><p>It's not hard to prove that there will be no paradox for <span class="tex-span"><i>c</i> = 0</span>. The situation may be worse for bigger <span class="tex-span"><i>c</i></span>. What is the maximum real value <span class="tex-span"><i>c</i></span> (remember that <img align="middle" class="tex-formula" src="file://hAiPDlhO.png" style="max-width: 100.0%;max-height: 100.0%;">) for which there is no paradox possible, that is, there will be no paradox for <span class="tex-font-style-bf">any optimal order</span> of solving problems?</p><p>It can be proved that the answer (the maximum <span class="tex-span"><i>c</i></span> as described) always exists.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150 000</span>)&nbsp;— the number of problems.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— initial scores.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the number of minutes needed to solve the <span class="tex-span"><i>i</i></span>-th problem.</p></div><div class="output-specification"><p>Print one real value on a single line&nbsp;— the maximum value of <span class="tex-span"><i>c</i></span> that <img align="middle" class="tex-formula" src="file://esxNGGEb.png" style="max-width: 100.0%;max-height: 100.0%;"> and there is no optimal order with a paradox. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://hKwJFZVA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 150 000</span>)&nbsp;— the number of problems.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— initial scores.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the number of minutes needed to solve the <span class="tex-span"><i>i</i></span>-th problem.</p>

## Output

<p>Print one real value on a single line&nbsp;— the maximum value of <span class="tex-span"><i>c</i></span> that <img align="middle" class="tex-formula" src="file://esxNGGEb.png" style="max-width: 100.0%;max-height: 100.0%;"> and there is no optimal order with a paradox. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <img align="middle" class="tex-formula" src="file://hKwJFZVA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3
4 3 10
1 1 8

```




```input2
4
7 20 15 10
7 20 15 10

```




```input3
2
10 20
10 1

```




```output1
0.62500000000

```




```output2
0.31901840491

```




```output3
1.00000000000

```



## Note

<p>In the first sample, there are <span class="tex-span">3</span> problems. The first is <span class="tex-span">(4, 1)</span> (initial score is <span class="tex-span">4</span> and required time is <span class="tex-span">1</span> minute), the second problem is <span class="tex-span">(3, 1)</span> and the third one is <span class="tex-span">(10, 8)</span>. The total time is <span class="tex-span"><i>T</i> = 1 + 1 + 8 = 10</span>.</p><p>Let's show that there is a paradox for <span class="tex-span"><i>c</i> = 0.7</span>. Solving problems in order <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> turns out to give the best total score, equal to the sum of:</p><ol> <li> solved <span class="tex-span">1</span> minute after the start: <img align="middle" class="tex-formula" src="file://CKtia9Qo.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> solved <span class="tex-span">2</span> minutes after the start: <img align="middle" class="tex-formula" src="file://f7dnAwEM.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> solved <span class="tex-span">10</span> minutes after the start: <img align="middle" class="tex-formula" src="file://huJtQSoh.png" style="max-width: 100.0%;max-height: 100.0%;"> </li></ol><p>So, this order gives <span class="tex-span">3.72 + 2.58 + 3 = 9.3</span> points in total and this is the only optimal order (you can calculate total scores for other <span class="tex-span">5</span> possible orders too see that they are lower). You should check points for problems <span class="tex-span">1</span> and <span class="tex-span">3</span> to see a paradox. There is <span class="tex-span">4 &lt; 10</span> but <span class="tex-span">3.72 &gt; 3</span>. It turns out that there is no paradox for <span class="tex-span"><i>c</i> = 0.625</span> but there is a paradox for any bigger <span class="tex-span"><i>c</i></span>.</p><p>In the second sample, all <span class="tex-span">24</span> orders are optimal.</p><p>In the third sample, even for <span class="tex-span"><i>c</i> = 1</span> there is no paradox.</p>
