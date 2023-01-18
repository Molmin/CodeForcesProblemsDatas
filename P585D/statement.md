## Description

<div><p>In the game Lizard Era: Beginning the protagonist will travel with three companions: Lynn, Meliana and Worrigan. Overall the game has <span class="tex-span"><i>n</i></span> mandatory quests. To perform each of them, you need to take <span class="tex-font-style-bf">exactly two</span> companions.</p><p>The attitude of each of the companions to the hero is an integer. Initially, the attitude of each of them to the hero of neutral and equal to 0. As the hero completes quests, he makes actions that change the attitude of the companions, whom he took to perform this task, in positive or negative direction.</p><p>Tell us what companions the hero needs to choose to make their attitude equal after completing all the quests. If this can be done in several ways, choose the one in which the value of resulting attitude is greatest possible.</p></div><div class="input-specification"><p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 25</span>) — the number of important tasks. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the tasks — the <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> — the values by which the attitude of Lynn, Meliana and Worrigan respectively will change towards the hero if the hero takes them on the <span class="tex-span"><i>i</i></span>-th task. All the numbers in the input are integers and do not exceed <span class="tex-span">10<sup class="upper-index">7</sup></span> in absolute value.</p></div><div class="output-specification"><p>If there is no solution, print in the first line "<span class="tex-font-style-tt">Impossible</span>".</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> lines, two characters is each line — in the <span class="tex-span"><i>i</i></span>-th line print the first letters of the companions' names that hero should take to complete the <span class="tex-span"><i>i</i></span>-th task ('<span class="tex-font-style-tt">L</span>' for Lynn, '<span class="tex-font-style-tt">M</span>' for Meliana, '<span class="tex-font-style-tt">W</span>' for Worrigan). Print the letters in any order, if there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 25</span>) — the number of important tasks. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the tasks — the <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>m</i><sub class="lower-index"><i>i</i></sub>, <i>w</i><sub class="lower-index"><i>i</i></sub></span> — the values by which the attitude of Lynn, Meliana and Worrigan respectively will change towards the hero if the hero takes them on the <span class="tex-span"><i>i</i></span>-th task. All the numbers in the input are integers and do not exceed <span class="tex-span">10<sup class="upper-index">7</sup></span> in absolute value.</p>

## Output

<p>If there is no solution, print in the first line "<span class="tex-font-style-tt">Impossible</span>".</p><p>Otherwise, print <span class="tex-span"><i>n</i></span> lines, two characters is each line — in the <span class="tex-span"><i>i</i></span>-th line print the first letters of the companions' names that hero should take to complete the <span class="tex-span"><i>i</i></span>-th task ('<span class="tex-font-style-tt">L</span>' for Lynn, '<span class="tex-font-style-tt">M</span>' for Meliana, '<span class="tex-font-style-tt">W</span>' for Worrigan). Print the letters in any order, if there are multiple solutions, print any of them.</p>





```input1
3
1 0 0
0 1 0
0 0 1

```




```input2
7
0 8 9
5 9 -2
6 -8 -7
9 4 5
-4 -9 9
-4 5 2
-6 8 -7

```




```input3
2
1 0 0
1 1 0

```




```output1
LM
MW
MW

```




```output2
LM
MW
LM
LW
MW
LM
LW

```




```output3
Impossible

```


