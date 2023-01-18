## Description

<div><p>A programming coach has <span class="tex-span"><i>n</i></span> students to teach. We know that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span">3</span>. Let's assume that all students are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive.</p><p>Before the university programming championship the coach wants to split all students into groups of three. For some pairs of students we know that they want to be on the same team. Besides, if the <span class="tex-span"><i>i</i></span>-th student wants to be on the same team with the <span class="tex-span"><i>j</i></span>-th one, then the <span class="tex-span"><i>j</i></span>-th student wants to be on the same team with the <span class="tex-span"><i>i</i></span>-th one. The coach wants the teams to show good results, so he wants the following condition to hold: if the <span class="tex-span"><i>i</i></span>-th student wants to be on the same team with the <span class="tex-span"><i>j</i></span>-th, then the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th students must be on the same team. Also, it is obvious that each student must be on exactly one team.</p><p>Help the coach and divide the teams the way he wants.</p></div><div class="input-specification"><p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 48</span>, <img align="middle" class="tex-formula" src="file://I9M29tqV.png" style="max-width: 100.0%;max-height: 100.0%;">. Then follow <span class="tex-span"><i>m</i></span> lines, each contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> means that students with numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> want to be on the same team.</p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span">3</span>. It is guaranteed that each pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> occurs in the input at most once.</p></div><div class="output-specification"><p>If the required division into teams doesn't exist, print number <span class="tex-font-style-tt">-1</span>. Otherwise, print <img align="middle" class="tex-formula" src="file://eKj6s4qy.png" style="max-width: 100.0%;max-height: 100.0%;"> lines. In each line print three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the <span class="tex-span"><i>i</i></span>-th team. </p><p>If there are multiple answers, you are allowed to print any of them.</p></div>

## Input

<p>The first line of the input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 48</span>, <img align="middle" class="tex-formula" src="file://I9M29tqV.png" style="max-width: 100.0%;max-height: 100.0%;">. Then follow <span class="tex-span"><i>m</i></span> lines, each contains a pair of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> means that students with numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> want to be on the same team.</p><p>It is guaranteed that <span class="tex-span"><i>n</i></span> is divisible by <span class="tex-span">3</span>. It is guaranteed that each pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> occurs in the input at most once.</p>

## Output

<p>If the required division into teams doesn't exist, print number <span class="tex-font-style-tt">-1</span>. Otherwise, print <img align="middle" class="tex-formula" src="file://eKj6s4qy.png" style="max-width: 100.0%;max-height: 100.0%;"> lines. In each line print three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the <span class="tex-span"><i>i</i></span>-th team. </p><p>If there are multiple answers, you are allowed to print any of them.</p>





```input1
3 0

```




```input2
6 4
1 2
2 3
3 4
5 6

```




```input3
3 3
1 2
2 3
1 3

```




```output1
3 2 1 

```




```output2
-1

```




```output3
3 2 1 

```


