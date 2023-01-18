## Description

<div><p>There is an automatic door at the entrance of a factory. The door works in the following way:</p><ul> <li> when one or several people come to the door and it is closed, the door immediately opens automatically and all people immediately come inside, </li><li> when one or several people come to the door and it is open, all people immediately come inside, </li><li> opened door immediately closes in <span class="tex-span"><i>d</i></span> seconds after its opening, </li><li> if the door is closing and one or several people are coming to the door at the same moment, then all of them will have enough time to enter and only after that the door will close. </li></ul><p>For example, if <span class="tex-span"><i>d</i> = 3</span> and four people are coming at four different moments of time <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> = 4</span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub> = 7</span>, <span class="tex-span"><i>t</i><sub class="lower-index">3</sub> = 9</span> and <span class="tex-span"><i>t</i><sub class="lower-index">4</sub> = 13</span> then the door will open three times: at moments <span class="tex-span">4</span>, <span class="tex-span">9</span> and <span class="tex-span">13</span>. It will close at moments <span class="tex-span">7</span> and <span class="tex-span">12</span>.</p><p>It is known that <span class="tex-span"><i>n</i></span> employees will enter at moments <span class="tex-span"><i>a</i>, 2·<i>a</i>, 3·<i>a</i>, ..., <i>n</i>·<i>a</i></span> (the value <span class="tex-span"><i>a</i></span> is positive integer). Also <span class="tex-span"><i>m</i></span> clients will enter at moments <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>m</i></sub></span>.</p><p>Write program to find the number of times the automatic door will open. Assume that the door is initially closed.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of the employees, the number of the clients, the moment of time when the first employee will come and the period of time in which the door closes.</p><p>The second line contains integer sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>) — moments of time when clients will come. The values <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are given in non-decreasing order.</p></div><div class="output-specification"><p>Print the number of times the door will open.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of the employees, the number of the clients, the moment of time when the first employee will come and the period of time in which the door closes.</p><p>The second line contains integer sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>) — moments of time when clients will come. The values <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are given in non-decreasing order.</p>

## Output

<p>Print the number of times the door will open.</p>





```input1
1 1 3 4
7

```




```input2
4 3 4 2
7 9 11

```




```output1
1

```




```output2
4

```



## Note

<p>In the first example the only employee will come at moment <span class="tex-span">3</span>. At this moment the door will open and will stay open until the moment <span class="tex-span">7</span>. At the same moment of time the client will come, so at first he will enter and only after it the door will close. Thus the door will open one time.</p>
