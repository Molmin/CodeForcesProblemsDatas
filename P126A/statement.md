## Description

<div><p>Bob is about to take a hot bath. </p><p>There are two taps to fill the bath: a hot water tap and a cold water tap. The cold water's temperature is <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, and the hot water's temperature is <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>. The cold water tap can transmit any integer number of water units per second from <span class="tex-span">0</span> to <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, inclusive. Similarly, the hot water tap can transmit from <span class="tex-span">0</span> to <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> water units per second.</p><p>If <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> water units per second flow through the first tap and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> water units per second flow through the second tap, then the resulting bath water temperature will be:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://g4gBK0LI.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Bob wants to open both taps so that the bath water temperature was not less than <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span>. However, the temperature should be as close as possible to this value. If there are several optimal variants, Bob chooses the one that lets fill the bath in the quickest way possible.</p><p>Determine how much each tap should be opened so that Bob was pleased with the result in the end.</p></div><div class="input-specification"><p>You are given five integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub> ≤ <i>t</i><sub class="lower-index">0</sub> ≤ <i>t</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>Print two space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>x</i><sub class="lower-index">2</sub></span>).</p></div>

## Input

<p>You are given five integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub> ≤ <i>t</i><sub class="lower-index">0</sub> ≤ <i>t</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>Print two space-separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> (<span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">1</sub> ≤ <i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span">0 ≤ <i>y</i><sub class="lower-index">2</sub> ≤ <i>x</i><sub class="lower-index">2</sub></span>).</p>





```input1
10 70 100 100 25

```




```input2
300 500 1000 1000 300

```




```input3
143 456 110 117 273

```




```output1
99 33
```




```output2
1000 0
```




```output3
76 54
```



## Note

<p>In the second sample the hot water tap shouldn't be opened, but the cold water tap should be opened at full capacity in order to fill the bath in the quickest way possible.</p>
