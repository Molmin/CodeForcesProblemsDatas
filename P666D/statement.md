## Description

<div><p>Group of Berland scientists, with whom you have a close business relationship, makes a research in the area of peaceful nuclear energy. In particular, they found that a group of four nanobots, placed on a surface of a plate, can run a powerful chain reaction under certain conditions. </p><p>To be precise, researchers introduced a rectangular Cartesian coordinate system on a flat plate and selected four distinct points with integer coordinates where bots will be placed initially. Next each bot will be assigned with one of the four directions (up, down, left or right) parallel to the coordinate axes. After that, each bot is shifted by an integer distance (which may be different for different bots) along its direction. The chain reaction starts, if the bots are in the corners of a square with <span class="tex-font-style-bf">positive area</span> with sides parallel to the coordinate axes. <span class="tex-font-style-bf">Each corner of the square must contain one nanobot.</span> This reaction will be stronger, if bots spend less time to move. We can assume that bots move with unit speed. In other words, the lesser is the maximum length traveled by bot, the stronger is reaction.</p><p>Scientists have prepared a set of plates and selected starting position for the bots for each plate. Now they ask you to assign the direction for each bot to move after <span class="tex-font-style-it">landing</span> such that the maximum length traveled by bot is as small as possible.</p></div><div class="input-specification"><p>The first line contains an integer number <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 50</span>) — the number of plates.</p><p><span class="tex-span"><i>t</i></span> descriptions of plates follow. A description of each plate consists of four lines. Each line consists of a pair of integers numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — coordinates of the next bot. All bots are in different locations.</p><p><span class="tex-font-style-it">Note, though, the problem can include several records in one test, you can hack other people's submissions only with the test of one plate, i.e. parameter <span class="tex-span"><i>t</i></span> in a hack test should be equal to <span class="tex-span">1</span>.</span></p></div><div class="output-specification"><p>Print answers for all plates separately. First goes a single integer number in a separate line. If scientists have made an unfortunate mistake and nanobots are not able to form the desired square, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum possible length of the longest bot's path.</p><p>If a solution exists, in the next four lines print two integer numbers — positions of each bot after moving. Print bots' positions in the order they are specified in the input data.</p><p>If there are multiple solution, you can print any of them.</p></div>

## Input

<p>The first line contains an integer number <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 50</span>) — the number of plates.</p><p><span class="tex-span"><i>t</i></span> descriptions of plates follow. A description of each plate consists of four lines. Each line consists of a pair of integers numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>) — coordinates of the next bot. All bots are in different locations.</p><p><span class="tex-font-style-it">Note, though, the problem can include several records in one test, you can hack other people's submissions only with the test of one plate, i.e. parameter <span class="tex-span"><i>t</i></span> in a hack test should be equal to <span class="tex-span">1</span>.</span></p>

## Output

<p>Print answers for all plates separately. First goes a single integer number in a separate line. If scientists have made an unfortunate mistake and nanobots are not able to form the desired square, print <span class="tex-font-style-tt">-1</span>. Otherwise, print the minimum possible length of the longest bot's path.</p><p>If a solution exists, in the next four lines print two integer numbers — positions of each bot after moving. Print bots' positions in the order they are specified in the input data.</p><p>If there are multiple solution, you can print any of them.</p>





```input1
2
1 1
1 -1
-1 1
-1 -1
1 1
2 2
4 4
6 6

```




```output1
0
1 1
1 -1
-1 1
-1 -1
-1

```


