## Description

<div><p>Tourist walks along the <span class="tex-span"><i>X</i></span> axis. He can choose either of two directions and any speed not exceeding <span class="tex-span"><i>V</i></span>. He can also stand without moving anywhere. He knows from newspapers that at time <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span> in the point with coordinate <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> an interesting event will occur, at time <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span> in the point with coordinate <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> — another one, and so on up to (<span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub>, <i>t</i><sub class="lower-index"><i>n</i></sub></span>). Interesting events are short so we can assume they are immediate. Event <span class="tex-span"><i>i</i></span> counts visited if at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> tourist was at point with coordinate <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Write program tourist that will find maximum number of events tourist if: </p><ul> <li> at the beginning (when time is equal to 0) tourist appears at point 0, </li><li> tourist can choose initial point for himself. </li></ul><p>Yes, you should answer on two similar but different questions.</p></div><div class="input-specification"><p>The first line of input contains single integer number <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100000</span>) — number of interesting events. The following <span class="tex-span"><i>N</i></span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — coordinate and time of the <span class="tex-span"><i>i</i></span>-th event. The last line of the input contains integer <span class="tex-span"><i>V</i></span> — maximum speed of the tourist. All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will be within range <span class="tex-span"> - 2·10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">8</sup></span>, all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> will be between <span class="tex-span">1</span> and <span class="tex-span">2·10<sup class="upper-index">6</sup></span> inclusive. <span class="tex-span"><i>V</i></span> will be positive and will not exceed 1000. The input may contain events that happen at the same time or in the same place but not in the same place at the same time.</p></div><div class="output-specification"><p>The only line of the output should contain two space-sepatated integers — maximum number of events tourist can visit in he starts moving from point 0 at time 0, and maximum number of events tourist can visit if he chooses the initial point for himself.</p></div>

## Input

<p>The first line of input contains single integer number <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 100000</span>) — number of interesting events. The following <span class="tex-span"><i>N</i></span> lines contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — coordinate and time of the <span class="tex-span"><i>i</i></span>-th event. The last line of the input contains integer <span class="tex-span"><i>V</i></span> — maximum speed of the tourist. All <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> will be within range <span class="tex-span"> - 2·10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">8</sup></span>, all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> will be between <span class="tex-span">1</span> and <span class="tex-span">2·10<sup class="upper-index">6</sup></span> inclusive. <span class="tex-span"><i>V</i></span> will be positive and will not exceed 1000. The input may contain events that happen at the same time or in the same place but not in the same place at the same time.</p>

## Output

<p>The only line of the output should contain two space-sepatated integers — maximum number of events tourist can visit in he starts moving from point 0 at time 0, and maximum number of events tourist can visit if he chooses the initial point for himself.</p>





```input1
3
-1 1
42 7
40 8
2

```




```output1
1 2

```


