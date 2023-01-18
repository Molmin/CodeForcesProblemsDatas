## Description

<div><p>The School №0 of the capital of Berland has <span class="tex-span"><i>n</i></span> children studying in it. All the children in this school are gifted: some of them are good at programming, some are good at maths, others are good at PE (Physical Education). Hence, for each child we know value <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>:</p><ul> <li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, if the <span class="tex-span"><i>i</i></span>-th child is good at programming, </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, if the <span class="tex-span"><i>i</i></span>-th child is good at maths, </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 3</span>, if the <span class="tex-span"><i>i</i></span>-th child is good at PE </li></ul><p>Each child happens to be good at exactly one of these three subjects.</p><p>The Team Scientific Decathlon Olympias requires teams of three students. The school teachers decided that the teams will be composed of three children that are good at different subjects. That is, each team must have one mathematician, one programmer and one sportsman. Of course, each child can be a member of no more than one team.</p><p>What is the maximum number of teams that the school will be able to present at the Olympiad? How should the teams be formed for that?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of children in the school. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> describes the skill of the <span class="tex-span"><i>i</i></span>-th child.</p></div><div class="output-specification"><p>In the first line output integer <span class="tex-span"><i>w</i></span> — the largest possible number of teams. </p><p>Then print <span class="tex-span"><i>w</i></span> lines, containing three numbers in each line. Each triple represents the indexes of the children forming the team. You can print both the teams, and the numbers in the triplets in any order. The children are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order of their appearance in the input. Each child must participate in no more than one team. If there are several solutions, print any of them.</p><p>If no teams can be compiled, print the only line with value <span class="tex-span"><i>w</i></span> equal to 0.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the number of children in the school. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> describes the skill of the <span class="tex-span"><i>i</i></span>-th child.</p>

## Output

<p>In the first line output integer <span class="tex-span"><i>w</i></span> — the largest possible number of teams. </p><p>Then print <span class="tex-span"><i>w</i></span> lines, containing three numbers in each line. Each triple represents the indexes of the children forming the team. You can print both the teams, and the numbers in the triplets in any order. The children are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order of their appearance in the input. Each child must participate in no more than one team. If there are several solutions, print any of them.</p><p>If no teams can be compiled, print the only line with value <span class="tex-span"><i>w</i></span> equal to 0.</p>





```input1
7
1 3 1 3 2 1 2

```




```input2
4
2 1 1 2

```




```output1
2
3 5 2
6 7 4

```




```output2
0

```


