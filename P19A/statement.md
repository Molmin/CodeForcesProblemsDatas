## Description

<div><p>Everyone knows that 2010 FIFA World Cup is being held in South Africa now. By the decision of BFA (Berland's Football Association) next World Cup will be held in Berland. BFA took the decision to change some World Cup regulations:</p><ul> <li> the final tournament features <span class="tex-span"><i>n</i></span> teams (<span class="tex-span"><i>n</i></span> is always even) </li><li> the first <span class="tex-span"><i>n</i> / 2</span> teams (according to the standings) come through to the knockout stage </li><li> the standings are made on the following principle: for a victory a team gets 3 points, for a draw — 1 point, for a defeat — 0 points. In the first place, teams are ordered in the standings in decreasing order of their points; in the second place — in decreasing order of the difference between scored and missed goals; in the third place — in the decreasing order of scored goals </li><li> it's written in Berland's Constitution that the previous regulation helps to order the teams without ambiguity. </li></ul><p>You are asked to write a program that, by the given list of the competing teams and the results of all the matches, will find the list of teams that managed to get through to the knockout stage.</p></div><div class="input-specification"><p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — amount of the teams, taking part in the final tournament of World Cup. The following <span class="tex-span"><i>n</i></span> lines contain the names of these teams, a name is a string of lower-case and upper-case Latin letters, its length doesn't exceed 30 characters. The following <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> lines describe the held matches in the format <span class="tex-font-style-tt">name1-name2 num1:num2</span>, where <span class="tex-span"><i>name</i>1</span>, <span class="tex-span"><i>name</i>2</span> — names of the teams; <span class="tex-span"><i>num</i>1</span>, <span class="tex-span"><i>num</i>2</span> (<span class="tex-span">0 ≤ <i>num</i>1, <i>num</i>2 ≤ 100</span>) — amount of the goals, scored by the corresponding teams. Accuracy of the descriptions is guaranteed: there are no two team names coinciding accurate to the letters' case; there is no match, where a team plays with itself; each match is met in the descriptions only once.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i> / 2</span> lines — names of the teams, which managed to get through to the knockout stage in lexicographical order. Output each name in a separate line. No odd characters (including spaces) are allowed. It's guaranteed that the described regulations help to order the teams without ambiguity.</p></div>

## Input

<p>The first input line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — amount of the teams, taking part in the final tournament of World Cup. The following <span class="tex-span"><i>n</i></span> lines contain the names of these teams, a name is a string of lower-case and upper-case Latin letters, its length doesn't exceed 30 characters. The following <span class="tex-span"><i>n</i>·(<i>n</i> - 1) / 2</span> lines describe the held matches in the format <span class="tex-font-style-tt">name1-name2 num1:num2</span>, where <span class="tex-span"><i>name</i>1</span>, <span class="tex-span"><i>name</i>2</span> — names of the teams; <span class="tex-span"><i>num</i>1</span>, <span class="tex-span"><i>num</i>2</span> (<span class="tex-span">0 ≤ <i>num</i>1, <i>num</i>2 ≤ 100</span>) — amount of the goals, scored by the corresponding teams. Accuracy of the descriptions is guaranteed: there are no two team names coinciding accurate to the letters' case; there is no match, where a team plays with itself; each match is met in the descriptions only once.</p>

## Output

<p>Output <span class="tex-span"><i>n</i> / 2</span> lines — names of the teams, which managed to get through to the knockout stage in lexicographical order. Output each name in a separate line. No odd characters (including spaces) are allowed. It's guaranteed that the described regulations help to order the teams without ambiguity.</p>





```input1
4
A
B
C
D
A-B 1:1
A-C 2:2
A-D 1:0
B-C 1:0
B-D 0:3
C-D 0:3

```




```input2
2
a
A
a-A 2:1

```




```output1
A
D

```




```output2
a

```


