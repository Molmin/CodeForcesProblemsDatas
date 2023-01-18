## Description

<div><p>Sasha and Kolya decided to get drunk with Coke, again. This time they have <span class="tex-span"><i>k</i></span> types of Coke. <span class="tex-span"><i>i</i></span>-th type is characterised by its carbon dioxide concentration <img align="middle" class="tex-formula" src="file://ttVMm04S.png" style="max-width: 100.0%;max-height: 100.0%;">. Today, on the party in honour of Sergiy of Vancouver they decided to prepare a glass of Coke with carbon dioxide concentration <img align="middle" class="tex-formula" src="file://73CaSFCT.png" style="max-width: 100.0%;max-height: 100.0%;">. The drink should also be tasty, so the glass can contain only integer number of liters of each Coke type (some types can be not presented in the glass). Also, they want to minimize the total volume of Coke in the glass.</p><p>Carbon dioxide concentration is defined as the volume of carbone dioxide in the Coke divided by the total volume of Coke. When you mix two Cokes, the volume of carbon dioxide sums up, and the total volume of Coke sums up as well.</p><p>Help them, find the minimal natural number of liters needed to create a glass with carbon dioxide concentration <img align="middle" class="tex-formula" src="file://7SU6zQTV.png" style="max-width: 100.0%;max-height: 100.0%;">. Assume that the friends have unlimited amount of each Coke type.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— carbon dioxide concentration the friends want and the number of Coke types.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— carbon dioxide concentration of each type of Coke. Some Coke types can have same concentration.</p></div><div class="output-specification"><p>Print the minimal natural number of liter needed to prepare a glass with carbon dioxide concentration <img align="middle" class="tex-formula" src="file://FMuEB1l5.png" style="max-width: 100.0%;max-height: 100.0%;">, or <span class="tex-font-style-tt">-1</span> if it is impossible.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— carbon dioxide concentration the friends want and the number of Coke types.</p><p>The second line contains <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— carbon dioxide concentration of each type of Coke. Some Coke types can have same concentration.</p>

## Output

<p>Print the minimal natural number of liter needed to prepare a glass with carbon dioxide concentration <img align="middle" class="tex-formula" src="file://FMuEB1l5.png" style="max-width: 100.0%;max-height: 100.0%;">, or <span class="tex-font-style-tt">-1</span> if it is impossible.</p>





```input1
400 4
100 300 450 500

```




```input2
50 2
100 25

```




```output1
2

```




```output2
3

```



## Note

<p>In the first sample case, we can achieve concentration <img align="middle" class="tex-formula" src="file://xmSKfTjp.png" style="max-width: 100.0%;max-height: 100.0%;"> using one liter of Coke of types <img align="middle" class="tex-formula" src="file://AFzcC40q.png" style="max-width: 100.0%;max-height: 100.0%;"> and <img align="middle" class="tex-formula" src="file://4koXDokn.png" style="max-width: 100.0%;max-height: 100.0%;">: <img align="middle" class="tex-formula" src="file://1w2YZsXD.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second case, we can achieve concentration <img align="middle" class="tex-formula" src="file://vrPJ44X2.png" style="max-width: 100.0%;max-height: 100.0%;"> using two liters of <img align="middle" class="tex-formula" src="file://kwxxrss8.png" style="max-width: 100.0%;max-height: 100.0%;"> type and one liter of <img align="middle" class="tex-formula" src="file://Na4Ic6TB.png" style="max-width: 100.0%;max-height: 100.0%;"> type: <img align="middle" class="tex-formula" src="file://L00hjIs8.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
