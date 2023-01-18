## Description

<div><p>General Payne has a battalion of <span class="tex-span"><i>n</i></span> soldiers. The soldiers' beauty contest is coming up, it will last for <span class="tex-span"><i>k</i></span> days. Payne decided that his battalion will participate in the pageant. Now he has choose the participants.</p><p>All soldiers in the battalion have different beauty that is represented by a positive integer. The value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the beauty of the <span class="tex-span"><i>i</i></span>-th soldier.</p><p>On each of <span class="tex-span"><i>k</i></span> days Generals has to send a detachment of soldiers to the pageant. The beauty of the detachment is the sum of the beauties of the soldiers, who are part of this detachment. Payne wants to surprise the jury of the beauty pageant, so each of <span class="tex-span"><i>k</i></span> days the beauty of the sent detachment should be unique. In other words, all <span class="tex-span"><i>k</i></span> beauties of the sent detachments must be distinct numbers.</p><p>Help Payne choose <span class="tex-span"><i>k</i></span> detachments of different beauties for the pageant. Please note that Payne cannot just forget to send soldiers on one day, that is, the detachment of soldiers he sends to the pageant should never be empty.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>; <span class="tex-span">1 ≤ <i>k</i> ≤ </span> <img align="middle" class="tex-formula" src="file://zaGGJWZs.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of soldiers and the number of days in the pageant, correspondingly. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span> — the beauties of the battalion soldiers.</p><p>It is guaranteed that Payne's battalion doesn't have two soldiers with the same beauty.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th line print the description of the detachment that will participate in the pageant on the <span class="tex-span"><i>i</i></span>-th day. The description consists of integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the number of soldiers in the detachment on the <span class="tex-span"><i>i</i></span>-th day of the pageant and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1, <i>i</i></sub>, <i>p</i><sub class="lower-index">2, <i>i</i></sub>, ..., <i>p</i><sub class="lower-index"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>i</i></sub></span> — the beauties of the soldiers in the detachment on the <span class="tex-span"><i>i</i></span>-th day of the pageant. The beauties of the soldiers are allowed to print in any order.</p><p>Separate numbers on the lines by spaces. It is guaranteed that there is the solution that meets the problem conditions. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>; <span class="tex-span">1 ≤ <i>k</i> ≤ </span> <img align="middle" class="tex-formula" src="file://zaGGJWZs.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of soldiers and the number of days in the pageant, correspondingly. The second line contains space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup>)</span> — the beauties of the battalion soldiers.</p><p>It is guaranteed that Payne's battalion doesn't have two soldiers with the same beauty.</p>

## Output

<p>Print <span class="tex-span"><i>k</i></span> lines: in the <span class="tex-span"><i>i</i></span>-th line print the description of the detachment that will participate in the pageant on the <span class="tex-span"><i>i</i></span>-th day. The description consists of integer <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the number of soldiers in the detachment on the <span class="tex-span"><i>i</i></span>-th day of the pageant and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1, <i>i</i></sub>, <i>p</i><sub class="lower-index">2, <i>i</i></sub>, ..., <i>p</i><sub class="lower-index"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>i</i></sub></span> — the beauties of the soldiers in the detachment on the <span class="tex-span"><i>i</i></span>-th day of the pageant. The beauties of the soldiers are allowed to print in any order.</p><p>Separate numbers on the lines by spaces. It is guaranteed that there is the solution that meets the problem conditions. If there are multiple solutions, print any of them.</p>





```input1
3 3
1 2 3

```




```input2
2 1
7 12

```




```output1
1 1
1 2
2 3 2

```




```output2
1 12 

```


