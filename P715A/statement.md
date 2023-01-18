## Description

<div><p>ZS the Coder is playing a game. There is a number displayed on the screen and there are two buttons, '<span class="tex-span"> + </span>' (plus) and '<img align="middle" class="tex-formula" src="file://P40TMOJC.png" style="max-width: 100.0%;max-height: 100.0%;">' (square root). Initially, the number <span class="tex-span">2</span> is displayed on the screen. There are <span class="tex-span"><i>n</i> + 1</span> levels in the game and ZS the Coder start at the level <span class="tex-span">1</span>.</p><p>When ZS the Coder is at level <span class="tex-span"><i>k</i></span>, he can :</p><ol> <li> <span class="tex-font-style-it">Press the '<span class="tex-span"> + </span>' button</span>. This increases the number on the screen by exactly <span class="tex-span"><i>k</i></span>. So, if the number on the screen was <span class="tex-span"><i>x</i></span>, it becomes <span class="tex-span"><i>x</i> + <i>k</i></span>.</li><li> <span class="tex-font-style-it">Press the '<img align="middle" class="tex-formula" src="file://0QzSzIZk.png" style="max-width: 100.0%;max-height: 100.0%;">' button</span>. Let the number on the screen be <span class="tex-span"><i>x</i></span>. After pressing this button, the number becomes <img align="middle" class="tex-formula" src="file://QwrBmJ82.png" style="max-width: 100.0%;max-height: 100.0%;">. After that, ZS the Coder levels up, so his current level becomes <span class="tex-span"><i>k</i> + 1</span>. This button can only be pressed when <span class="tex-span"><i>x</i></span> is a <span class="tex-font-style-bf">perfect square</span>, i.e. <span class="tex-span"><i>x</i> = <i>m</i><sup class="upper-index">2</sup></span> for some positive integer <span class="tex-span"><i>m</i></span>. </li></ol><p>Additionally, after each move, if ZS the Coder is at level <span class="tex-span"><i>k</i></span>, and the number on the screen is <span class="tex-span"><i>m</i></span>, then <span class="tex-font-style-bf"><span class="tex-span"><i>m</i></span> must be a multiple of <span class="tex-span"><i>k</i></span></span>. Note that this condition is only checked after performing the press. For example, if ZS the Coder is at level <span class="tex-span">4</span> and current number is <span class="tex-span">100</span>, he presses the '<img align="middle" class="tex-formula" src="file://UnRwwsFU.png" style="max-width: 100.0%;max-height: 100.0%;">' button and the number turns into <span class="tex-span">10</span>. Note that at this moment, <span class="tex-span">10</span> is not divisible by <span class="tex-span">4</span>, but this press is still valid, because after it, ZS the Coder is at level <span class="tex-span">5</span>, and <span class="tex-span">10</span> is divisible by <span class="tex-span">5</span>.</p><p>ZS the Coder needs your help in beating the game&nbsp;— he wants to reach level <span class="tex-span"><i>n</i> + 1</span>. In other words, he needs to press the '<img align="middle" class="tex-formula" src="file://iV06CthQ.png" style="max-width: 100.0%;max-height: 100.0%;">' button <span class="tex-span"><i>n</i></span> times. Help him determine the number of times he should press the '<span class="tex-span"> + </span>' button before pressing the '<img align="middle" class="tex-formula" src="file://SBYHoTWv.png" style="max-width: 100.0%;max-height: 100.0%;">' button at each level. </p><p>Please note that ZS the Coder wants to find just any sequence of presses allowing him to reach level <span class="tex-span"><i>n</i> + 1</span>, but not necessarily a sequence minimizing the number of presses.</p></div><div class="input-specification"><p>The first and only line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>), denoting that ZS the Coder wants to reach level <span class="tex-span"><i>n</i> + 1</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> non-negative integers, one per line. <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of times that ZS the Coder needs to press the '<span class="tex-span"> + </span>' button before pressing the '<img align="middle" class="tex-formula" src="file://rMU1OGi6.png" style="max-width: 100.0%;max-height: 100.0%;">' button at level <span class="tex-span"><i>i</i></span>. </p><p>Each number in the output should not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>. However, the number on the screen <span class="tex-font-style-bf">can be greater</span> than <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p><p>It is guaranteed that at least one solution exists. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first and only line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>), denoting that ZS the Coder wants to reach level <span class="tex-span"><i>n</i> + 1</span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> non-negative integers, one per line. <span class="tex-span"><i>i</i></span>-th of them should be equal to the number of times that ZS the Coder needs to press the '<span class="tex-span"> + </span>' button before pressing the '<img align="middle" class="tex-formula" src="file://rMU1OGi6.png" style="max-width: 100.0%;max-height: 100.0%;">' button at level <span class="tex-span"><i>i</i></span>. </p><p>Each number in the output should not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>. However, the number on the screen <span class="tex-font-style-bf">can be greater</span> than <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p><p>It is guaranteed that at least one solution exists. If there are multiple solutions, print any of them.</p>





```input1
3

```




```input2
2

```




```input3
4

```




```output1
14
16
46

```




```output2
999999999999999998
44500000000

```




```output3
2
17
46
97

```



## Note

<p>In the first sample case:</p><p>On the first level, ZS the Coder pressed the '<span class="tex-span"> + </span>' button <span class="tex-span">14</span> times (and the number on screen is initially <span class="tex-span">2</span>), so the number became <span class="tex-span">2 + 14·1 = 16</span>. Then, ZS the Coder pressed the '<img align="middle" class="tex-formula" src="file://TFA93vqm.png" style="max-width: 100.0%;max-height: 100.0%;">' button, and the number became <img align="middle" class="tex-formula" src="file://UIyaiNsu.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>After that, on the second level, ZS pressed the '<span class="tex-span"> + </span>' button <span class="tex-span">16</span> times, so the number becomes <span class="tex-span">4 + 16·2 = 36</span>. Then, ZS pressed the '<img align="middle" class="tex-formula" src="file://WoNA7Ph9.png" style="max-width: 100.0%;max-height: 100.0%;">' button, levelling up and changing the number into <img align="middle" class="tex-formula" src="file://WFM9fHbd.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>After that, on the third level, ZS pressed the '<span class="tex-span"> + </span>' button <span class="tex-span">46</span> times, so the number becomes <span class="tex-span">6 + 46·3 = 144</span>. Then, ZS pressed the '<img align="middle" class="tex-formula" src="file://nVZo2fYZ.png" style="max-width: 100.0%;max-height: 100.0%;">' button, levelling up and changing the number into <img align="middle" class="tex-formula" src="file://h3vJyfcm.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Note that <span class="tex-span">12</span> is indeed divisible by <span class="tex-span">4</span>, so ZS the Coder can reach level <span class="tex-span">4</span>.</p><p>Also, note that pressing the '<span class="tex-span"> + </span>' button <span class="tex-span">10</span> times on the third level before levelling up does not work, because the number becomes <span class="tex-span">6 + 10·3 = 36</span>, and when the '<img align="middle" class="tex-formula" src="file://3CyBGURA.png" style="max-width: 100.0%;max-height: 100.0%;">' button is pressed, the number becomes <img align="middle" class="tex-formula" src="file://YeJYcoHn.png" style="max-width: 100.0%;max-height: 100.0%;"> and ZS the Coder is at Level <span class="tex-span">4</span>. However, <span class="tex-span">6</span> is not divisible by <span class="tex-span">4</span> now, so this is <span class="tex-font-style-bf">not a valid solution.</span></p><p>In the second sample case:</p><p>On the first level, ZS the Coder pressed the '<span class="tex-span"> + </span>' button <span class="tex-span">999999999999999998</span> times (and the number on screen is initially <span class="tex-span">2</span>), so the number became <span class="tex-span">2 + 999999999999999998·1 = 10<sup class="upper-index">18</sup></span>. Then, ZS the Coder pressed the '<img align="middle" class="tex-formula" src="file://FF4DtW1e.png" style="max-width: 100.0%;max-height: 100.0%;">' button, and the number became <img align="middle" class="tex-formula" src="file://C0s0epHu.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>After that, on the second level, ZS pressed the '<span class="tex-span"> + </span>' button <span class="tex-span">44500000000</span> times, so the number becomes <span class="tex-span">10<sup class="upper-index">9</sup> + 44500000000·2 = 9·10<sup class="upper-index">10</sup></span>. Then, ZS pressed the '<img align="middle" class="tex-formula" src="file://rf4UbQYt.png" style="max-width: 100.0%;max-height: 100.0%;">' button, levelling up and changing the number into <img align="middle" class="tex-formula" src="file://DhHBA3oH.png" style="max-width: 100.0%;max-height: 100.0%;">. </p><p>Note that <span class="tex-span">300000</span> is a multiple of <span class="tex-span">3</span>, so ZS the Coder can reach level <span class="tex-span">3</span>.</p>
