## Description

<div><p>Inna loves sleeping very much, so she needs <span class="tex-span"><i>n</i></span> alarm clocks in total to wake up. Let's suppose that Inna's room is a <span class="tex-span">100 × 100</span> square with the lower left corner at point <span class="tex-span">(0, 0)</span> and with the upper right corner at point <span class="tex-span">(100, 100)</span>. Then the alarm clocks are points with integer coordinates in this square.</p><p>The morning has come. All <span class="tex-span"><i>n</i></span> alarm clocks in Inna's room are ringing, so Inna wants to turn them off. For that Inna has come up with an amusing game:</p><ul> <li> First Inna chooses a type of segments that she will use throughout the game. The segments can be either vertical or horizontal. </li><li> Then Inna makes multiple moves. In a single move, Inna can paint a segment of any length on the plane, she chooses its type at the beginning of the game (either vertical or horizontal), then all alarm clocks that are on this segment switch off. The game ends when all the alarm clocks are switched off. </li></ul><p>Inna is very sleepy, so she wants to get through the alarm clocks as soon as possible. Help her, find the minimum number of moves in the game that she needs to turn off all the alarm clocks!</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the alarm clocks. The next <span class="tex-span"><i>n</i></span> lines describe the clocks: the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th alarm clock <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p><p>Note that a single point in the room can contain any number of alarm clocks and the alarm clocks can lie on the sides of the square that represents the room.</p></div><div class="output-specification"><p>In a single line print a single integer — the minimum number of segments Inna will have to draw if she acts optimally.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the alarm clocks. The next <span class="tex-span"><i>n</i></span> lines describe the clocks: the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> — the coordinates of the <span class="tex-span"><i>i</i></span>-th alarm clock <span class="tex-span">(0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p><p>Note that a single point in the room can contain any number of alarm clocks and the alarm clocks can lie on the sides of the square that represents the room.</p>

## Output

<p>In a single line print a single integer — the minimum number of segments Inna will have to draw if she acts optimally.</p>





```input1
4
0 0
0 1
0 2
1 0

```




```input2
4
0 0
0 1
1 0
1 1

```




```input3
4
1 1
1 2
2 3
3 3

```




```output1
2

```




```output2
2

```




```output3
3

```



## Note

<p>In the first sample, Inna first chooses type "vertical segments", and then she makes segments with ends at : <span class="tex-span">(0, 0)</span>, <span class="tex-span">(0, 2)</span>; and, for example, <span class="tex-span">(1, 0)</span>, <span class="tex-span">(1, 1)</span>. If she paints horizontal segments, she will need at least 3 segments.</p><p>In the third sample it is important to note that Inna doesn't have the right to change the type of the segments during the game. That's why she will need 3 horizontal or 3 vertical segments to end the game.</p>
