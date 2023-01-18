## Description

<div><p>There is a programing contest named SnakeUp, <span class="tex-span">2<i>n</i></span> people want to compete for it. In order to attend this contest, people need to form teams of exactly two people. You are given the strength of each possible combination of two people. All the values of the strengths are <span class="tex-font-style-bf">distinct</span>.</p><p>Every contestant hopes that he can find a teammate so that their team’s strength is as high as possible. That is, a contestant will form a team with highest strength possible by choosing a teammate from ones who are willing to be a teammate with him/her. More formally, two people <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> may form a team if each of them is the best possible teammate (among the contestants that remain unpaired) for the other one. </p><p>Can you determine who will be each person’s teammate?</p></div><div class="input-specification"><p>There are <span class="tex-span">2<i>n</i></span> lines in the input. </p><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 400</span>) — the number of teams to be formed.</p><p>The <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span"><i>i</i> &gt; 1</span>) contains <span class="tex-span"><i>i</i> - 1</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>2</sub></span>, ... , <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>(<i>i</i> - 1)</sub></span>. Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, all <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> are distinct) denotes the strength of a team consisting of person <span class="tex-span"><i>i</i></span> and person <span class="tex-span"><i>j</i></span> (people are numbered starting from <span class="tex-span">1</span>.)</p></div><div class="output-specification"><p>Output a line containing <span class="tex-span">2<i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th number should represent the number of teammate of <span class="tex-span"><i>i</i></span>-th person.</p></div>

## Input

<p>There are <span class="tex-span">2<i>n</i></span> lines in the input. </p><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 400</span>) — the number of teams to be formed.</p><p>The <span class="tex-span"><i>i</i></span>-th line (<span class="tex-span"><i>i</i> &gt; 1</span>) contains <span class="tex-span"><i>i</i> - 1</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>2</sub></span>, ... , <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>(<i>i</i> - 1)</sub></span>. Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>ij</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, all <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> are distinct) denotes the strength of a team consisting of person <span class="tex-span"><i>i</i></span> and person <span class="tex-span"><i>j</i></span> (people are numbered starting from <span class="tex-span">1</span>.)</p>

## Output

<p>Output a line containing <span class="tex-span">2<i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th number should represent the number of teammate of <span class="tex-span"><i>i</i></span>-th person.</p>





```input1
2
6
1 2
3 4 5

```




```input2
3
487060
3831 161856
845957 794650 976977
83847 50566 691206 498447
698377 156232 59015 382455 626960

```




```output1
2 1 4 3

```




```output2
6 5 4 3 2 1

```



## Note

<p>In the first sample, contestant <span class="tex-span">1</span> and <span class="tex-span">2</span> will be teammates and so do contestant <span class="tex-span">3</span> and <span class="tex-span">4</span>, so the teammate of contestant <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> will be <span class="tex-span">2</span>, <span class="tex-span">1</span>, <span class="tex-span">4</span>, <span class="tex-span">3</span> respectively.</p>
