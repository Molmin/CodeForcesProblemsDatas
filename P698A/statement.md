## Description

<div><p>Vasya has <span class="tex-span"><i>n</i></span> days of vacations! So he decided to improve his IT skills and do sport. Vasya knows the following information about each of this <span class="tex-span"><i>n</i></span> days: whether that gym opened and whether a contest was carried out in the Internet on that day. For the <span class="tex-span"><i>i</i></span>-th day there are four options:</p><ol> <li> on this day the gym is closed and the contest is not carried out; </li><li> on this day the gym is closed and the contest is carried out; </li><li> on this day the gym is open and the contest is not carried out; </li><li> on this day the gym is open and the contest is carried out. </li></ol><p>On each of days Vasya can either have a rest or write the contest (if it is carried out on this day), or do sport (if the gym is open on this day).</p><p>Find the minimum number of days on which Vasya will have a rest (it means, he will not do sport and write the contest at the same time). The only limitation that Vasya has — <span class="tex-font-style-it">he does not want to do the same activity on two consecutive days: it means, he will not do sport on two consecutive days, and write the contest on two consecutive days</span>.</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of days of Vasya's vacations.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) separated by space, where: </p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 0, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is closed and the contest is not carried out; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 1, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is closed, but the contest is carried out; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 2, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is open and the contest is not carried out; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 3, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is open and the contest is carried out.</li></ul></div><div class="output-specification"><p>Print the minimum possible number of days on which Vasya will have a rest. Remember that Vasya refuses:</p><ul> <li> to do sport on any two consecutive days, </li><li> to write the contest on any two consecutive days. </li></ul></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of days of Vasya's vacations.</p><p>The second line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>) separated by space, where: </p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 0, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is closed and the contest is not carried out; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 1, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is closed, but the contest is carried out; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 2, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is open and the contest is not carried out; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 3, if on the <span class="tex-span"><i>i</i></span>-th day of vacations the gym is open and the contest is carried out.</li></ul>

## Output

<p>Print the minimum possible number of days on which Vasya will have a rest. Remember that Vasya refuses:</p><ul> <li> to do sport on any two consecutive days, </li><li> to write the contest on any two consecutive days. </li></ul>





```input1
4
1 3 2 0

```




```input2
7
1 3 3 2 1 2 3

```




```input3
2
2 2

```




```output1
2

```




```output2
0

```




```output3
1

```



## Note

<p>In the first test Vasya can write the contest on the day number 1 and do sport on the day number 3. Thus, he will have a rest for only 2 days.</p><p>In the second test Vasya should write contests on days number 1, 3, 5 and 7, in other days do sport. Thus, he will not have a rest for a single day.</p><p>In the third test Vasya can do sport either on a day number 1 or number 2. He can not do sport in two days, because it will be contrary to the his limitation. Thus, he will have a rest for only one day.</p>
