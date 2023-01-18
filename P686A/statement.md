## Description

<div><p>After their adventure with the magic mirror Kay and Gerda have returned home and sometimes give free ice cream to kids in the summer.</p><p>At the start of the day they have <span class="tex-span"><i>x</i></span> ice cream packs. Since the ice cream is free, people start standing in the queue before Kay and Gerda's house even in the night. Each person in the queue wants either to take several ice cream packs for himself and his friends or to give several ice cream packs to Kay and Gerda (carriers that bring ice cream have to stand in the same queue).</p><p>If a carrier with <span class="tex-span"><i>d</i></span> ice cream packs comes to the house, then Kay and Gerda take all his packs. If a child who wants to take <span class="tex-span"><i>d</i></span> ice cream packs comes to the house, then Kay and Gerda will give him <span class="tex-span"><i>d</i></span> packs if they have enough ice cream, otherwise the child will get no ice cream at all and will leave in distress.</p><p>Kay wants to find the amount of ice cream they will have after all people will leave from the queue, and Gerda wants to find the number of distressed kids.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a character '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>', and an integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Record "<span class="tex-font-style-tt">+ </span><span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>" in <span class="tex-span"><i>i</i></span>-th line means that a carrier with <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> ice cream packs occupies <span class="tex-span"><i>i</i></span>-th place from the start of the queue, and record "<span class="tex-font-style-tt">- </span><span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>" means that a child who wants to take <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> packs stands in <span class="tex-span"><i>i</i></span>-th place.</p></div><div class="output-specification"><p>Print two space-separated integers&nbsp;— number of ice cream packs left after all operations, and number of kids that left the house in distress.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a character '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>', and an integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, separated by a space (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Record "<span class="tex-font-style-tt">+ </span><span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>" in <span class="tex-span"><i>i</i></span>-th line means that a carrier with <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> ice cream packs occupies <span class="tex-span"><i>i</i></span>-th place from the start of the queue, and record "<span class="tex-font-style-tt">- </span><span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>" means that a child who wants to take <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> packs stands in <span class="tex-span"><i>i</i></span>-th place.</p>

## Output

<p>Print two space-separated integers&nbsp;— number of ice cream packs left after all operations, and number of kids that left the house in distress.</p>





```input1
5 7
+ 5
- 10
- 20
+ 40
- 20

```




```input2
5 17
- 16
- 2
- 98
+ 100
- 98

```




```output1
22 1

```




```output2
3 2

```



## Note

<p>Consider the first sample.</p><ol> <li> Initially Kay and Gerda have <span class="tex-span">7</span> packs of ice cream. </li><li> Carrier brings <span class="tex-span">5</span> more, so now they have <span class="tex-span">12</span> packs. </li><li> A kid asks for <span class="tex-span">10</span> packs and receives them. There are only <span class="tex-span">2</span> packs remaining. </li><li> Another kid asks for <span class="tex-span">20</span> packs. Kay and Gerda do not have them, so the kid goes away distressed. </li><li> Carrier bring <span class="tex-span">40</span> packs, now Kay and Gerda have <span class="tex-span">42</span> packs. </li><li> Kid asks for <span class="tex-span">20</span> packs and receives them. There are <span class="tex-span">22</span> packs remaining. </li></ol>
