## Description

<div><p><span class="tex-font-style-it">East or west, home is best. That's why family reunion, the indispensable necessity of Lunar New Year celebration, is put in such a position.</span></p><p>After the reunion dinner, Little Tommy plays a game with the family. Here is a concise introduction to this game: </p><ol> <li> There is a sequence of <span class="tex-span"><i>n</i></span> non-negative integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> in the beginning. It is ruled that each integer in this sequence should be non-negative <span class="tex-font-style-bf">at any time</span>. </li><li> You can select two <span class="tex-font-style-bf">consecutive positive</span> integers in this sequence, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span>, and then decrease them by their minimum (i.&nbsp;e. <span class="tex-span"><i>min</i>(<i>p</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>), the cost of this operation is equal to <span class="tex-span"><i>min</i>(<i>p</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i> + 1</sub>)</span>. We call such operation as a <span class="tex-font-style-it">descension</span>. </li><li> The game immediately ends when there are no two consecutive positive integers. Your task is to end the game so that the total cost of your operations is as small as possible. </li></ol><p>Obviously, every game ends after at most <span class="tex-span"><i>n</i> - 1</span> descensions. Please share your solution of this game with the lowest cost.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>i</i> = 1, 2, ..., <i>n</i>)</span>.</p></div><div class="output-specification"><p>In the first line print one integer as the number of descensions <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ <i>n</i> - 1)</span>.</p><p>In the next <span class="tex-span"><i>m</i></span> lines print the descensions chronologically. More precisely, in each line of the next <span class="tex-span"><i>m</i></span> lines print one integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span> representing a descension would operate on <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> such that all the descensions could be utilized from top to bottom.</p><p>If there are many possible solutions to reach the minimal cost, print any of them.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>i</i> = 1, 2, ..., <i>n</i>)</span>.</p>

## Output

<p>In the first line print one integer as the number of descensions <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>m</i> ≤ <i>n</i> - 1)</span>.</p><p>In the next <span class="tex-span"><i>m</i></span> lines print the descensions chronologically. More precisely, in each line of the next <span class="tex-span"><i>m</i></span> lines print one integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span> representing a descension would operate on <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i> + 1</sub></span> such that all the descensions could be utilized from top to bottom.</p><p>If there are many possible solutions to reach the minimal cost, print any of them.</p>





```input1
4
2 1 3 1

```




```input2
5
2 2 1 3 1

```




```output1
2
1
3

```




```output2
3
2
1
4

```



## Note

<p>In the first sample, one possible best solution is <img align="middle" class="tex-formula" src="file://yG4NGSds.png" style="max-width: 100.0%;max-height: 100.0%;">, of which the cost is <span class="tex-span">1 + 1 = 2</span>.</p><p>In the second sample, one possible best solution is <img align="middle" class="tex-formula" src="file://zE7j41uL.png" style="max-width: 100.0%;max-height: 100.0%;">, of which the cost is <span class="tex-span">1 + 1 + 1 = 3</span>.</p>
