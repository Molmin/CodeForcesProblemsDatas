## Description

<div><p>Vasya participates in a ski race along the <span class="tex-span"><i>X</i></span> axis. The start is at point <span class="tex-span">0</span>, and the finish is at <span class="tex-span"><i>L</i></span>, that is, at a distance <span class="tex-span"><i>L</i></span> meters from the start in the positive direction of the axis. Vasya has been training so hard that he can run one meter in exactly one second.</p><p>Besides, there are <span class="tex-span"><i>n</i></span> take-off ramps on the track, each ramp is characterized by four numbers: </p><ul> <li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> represents the ramp's coordinate </li><li> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> represents from how many meters Vasya will land if he goes down this ramp </li><li> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> represents the flight time in seconds </li><li> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is the number, indicating for how many meters Vasya should gather speed to get ready and fly off the ramp. As Vasya gathers speed, he should ski on the snow (that is, he should not be flying), but his speed still equals one meter per second. </li></ul><p>Vasya is allowed to move in <span class="tex-font-style-bf">any direction</span> on the <span class="tex-span"><i>X</i></span> axis, but he is prohibited to cross the start line, that is go to the negative semiaxis. Vasya himself chooses which take-off ramps he will use and in what order, that is, he is not obliged to take off from all the ramps he encounters. Specifically, Vasya can skip the ramp. It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>L</i></span>, that is, Vasya cannot cross the finish line in flight.</p><p><span class="tex-font-style-bf">Vasya can jump from the ramp only in the positive direction of <span class="tex-span"><i>X</i></span> axis. More formally, when using the <span class="tex-span"><i>i</i></span>-th ramp, Vasya starts gathering speed at point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> - <i>p</i><sub class="lower-index"><i>i</i></sub></span>, jumps at point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, and lands at point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub></span>. He cannot use the ramp in opposite direction.</span></p><p>Your task is to find the minimum time that Vasya will spend to cover the distance.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>L</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup></span>). Then <span class="tex-span"><i>n</i></span> lines contain the descriptions of the ramps, each description is on a single line. Each description is a group of four non-negative integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>L</i></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>L</i></span>).</p></div><div class="output-specification"><p>Print in the first line the minimum time in seconds Vasya needs to complete the track. Print in the second line <span class="tex-span"><i>k</i></span> — the number of take-off ramps that Vasya needs to use, and print on the third line of output <span class="tex-span"><i>k</i></span> numbers the number the take-off ramps Vasya used in the order in which he used them. Print each number exactly once, separate the numbers with a space. The ramps are numbered starting from 1 in the order in which they are given in the input.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>L</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>L</i> ≤ 10<sup class="upper-index">9</sup></span>). Then <span class="tex-span"><i>n</i></span> lines contain the descriptions of the ramps, each description is on a single line. Each description is a group of four non-negative integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>L</i></span>, <span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> + <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>L</i></span>).</p>

## Output

<p>Print in the first line the minimum time in seconds Vasya needs to complete the track. Print in the second line <span class="tex-span"><i>k</i></span> — the number of take-off ramps that Vasya needs to use, and print on the third line of output <span class="tex-span"><i>k</i></span> numbers the number the take-off ramps Vasya used in the order in which he used them. Print each number exactly once, separate the numbers with a space. The ramps are numbered starting from 1 in the order in which they are given in the input.</p>





```input1
2 20
5 10 5 5
4 16 1 7

```




```input2
2 20
9 8 12 6
15 5 1 1

```




```output1
15
1
1
```




```output2
16
1
2
```



## Note

<p>In the first sample, Vasya cannot use ramp 2, because then he will need to gather speed starting from point <span class="tex-font-style-tt">-3</span>, which is not permitted by the statement. The optimal option is using ramp 1, the resulting time is: moving to the point of gathering speed + gathering speed until reaching the takeoff ramp + flight time + moving to the finish line<span class="tex-span"> = 0 + 5 + 5 + 5 = 15</span>.</p><p>In the second sample using ramp 1 is not optimal for Vasya as <span class="tex-span"><i>t</i><sub class="lower-index">1</sub> &gt; <i>d</i><sub class="lower-index">1</sub></span>. The optimal option is using ramp 2, the resulting time is: moving to the point of gathering speed + gathering speed until reaching the takeoff ramp + flight time + moving to the finish line<span class="tex-span"> = 14 + 1 + 1 + 0 = 16</span>.</p>
