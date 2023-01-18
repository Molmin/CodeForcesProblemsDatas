## Description

<div><p>Have you ever tried to explain to the coordinator, why it is eight hours to the contest and not a single problem has been prepared yet? Misha had. And this time he has a <span class="tex-font-style-it">really</span> strong excuse: he faced a space-time paradox! Space and time replaced each other.</p><p>The entire universe turned into an enormous clock face with three hands&nbsp;— hour, minute, and second. Time froze, and clocks now show the time <span class="tex-span"><i>h</i></span> hours, <span class="tex-span"><i>m</i></span> minutes, <span class="tex-span"><i>s</i></span> seconds.</p><p>Last time Misha talked with the coordinator at <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> o'clock, so now he stands on the number <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> on the clock face. The contest should be ready by <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> o'clock. In the terms of paradox it means that Misha has to go to number <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> somehow. Note that he doesn't have to move forward only: in these circumstances time has no direction.</p><p>Clock hands are very long, and Misha cannot get round them. He also cannot step over as it leads to the collapse of space-time. That is, if hour clock points 12 and Misha stands at 11 then he cannot move to 1 along the top arc. He has to follow all the way round the clock center (of course, if there are no other hands on his way).</p><p>Given the hands' positions, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, and <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, find if Misha can prepare the contest on time (or should we say <span class="tex-font-style-it">on space</span>?). That is, find if he can move from <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> by the clock face.</p></div><div class="input-specification"><p>Five integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 12</span>, <span class="tex-span">0 ≤ <i>m</i>, <i>s</i> ≤ 59</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 12</span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> ≠ <i>t</i><sub class="lower-index">2</sub></span>).</p><p>Misha's position and the target time do not coincide with the position of any hand.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity), if Misha can prepare the contest on time, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each character either upper- or lowercase ("<span class="tex-font-style-tt">YeS</span>" and "<span class="tex-font-style-tt">yes</span>" are valid when the answer is "<span class="tex-font-style-tt">YES</span>").</p></div>

## Input

<p>Five integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>h</i> ≤ 12</span>, <span class="tex-span">0 ≤ <i>m</i>, <i>s</i> ≤ 59</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub> ≤ 12</span>, <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> ≠ <i>t</i><sub class="lower-index">2</sub></span>).</p><p>Misha's position and the target time do not coincide with the position of any hand.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (quotes for clarity), if Misha can prepare the contest on time, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each character either upper- or lowercase ("<span class="tex-font-style-tt">YeS</span>" and "<span class="tex-font-style-tt">yes</span>" are valid when the answer is "<span class="tex-font-style-tt">YES</span>").</p>





```input1
12 30 45 3 11

```




```input2
12 0 1 12 1

```




```input3
3 47 0 4 9

```




```output1
NO

```




```output2
YES

```




```output3
YES

```



## Note

<p>The three examples are shown on the pictures below from left to right. The starting position of Misha is shown with green, the ending position is shown with pink. Note that the positions of the hands on the pictures are not exact, but are close to the exact and the answer is the same.</p><center> <img class="tex-graphics" height="151px" src="file://cMnVCHRo.png" style="max-width: 100.0%;max-height: 100.0%;" width="476px"> </center>
