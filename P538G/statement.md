## Description

<div><p>Help! A robot escaped our lab and we need help finding it. </p><p>The lab is at the point <span class="tex-span">(0, 0)</span> of the coordinate plane, at time 0 the robot was there. The robot's movements are defined by a program&nbsp;— a string of length <span class="tex-span"><i>l</i></span>, consisting of characters <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">R</span>. Each second the robot executes the next command in his program: if the current coordinates of the robot are <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, then commands <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">R</span> move it to cells <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>, <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span>, <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span> respectively. The execution of the program started at time 0. The program is looped, i.e. each <span class="tex-span"><i>l</i></span> seconds of executing the program start again from the first character. Unfortunately, we don't know what program was loaded into the robot when he left the lab.</p><p>Our radars managed to find out the position of the robot at <span class="tex-span"><i>n</i></span> moments of time: we know that at the moment of time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> the robot is at the point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>. Given this data, either help to determine what program could be loaded into the robot, or determine that no possible program meets the data and the robot must have broken down.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 2·10<sup class="upper-index">6</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain three space-separated integers&nbsp;— <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">18</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>). The radar data is given chronologically, i.e. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i> - 1</span>.</p></div><div class="output-specification"><p>Print any of the possible programs that meet the data. If no program meets the data, print a single word '<span class="tex-font-style-tt">NO</span>' (without the quotes).</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>l</i> ≤ 2·10<sup class="upper-index">6</sup></span>).</p><p>Next <span class="tex-span"><i>n</i></span> lines contain three space-separated integers&nbsp;— <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"> - 10<sup class="upper-index">18</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>). The radar data is given chronologically, i.e. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>n</i> - 1</span>.</p>

## Output

<p>Print any of the possible programs that meet the data. If no program meets the data, print a single word '<span class="tex-font-style-tt">NO</span>' (without the quotes).</p>





```input1
3 3
1 1 0
2 1 -1
3 0 -1

```




```input2
2 2
1 1 0
999 1 0

```




```input3
2 5
10 10 0
20 0 0

```




```output1
RDL

```




```output2
RL

```




```output3
NO

```


