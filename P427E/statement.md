## Description

<div><p>Imagine that your city is an infinite 2D plane with Cartesian coordinate system. The only crime-affected road of your city is the <span class="tex-span"><i>x</i></span>-axis. Currently, there are <span class="tex-span"><i>n</i></span> criminals along the road. No police station has been built on this road yet, so the mayor wants to build one.</p><p>As you are going to be in charge of this new police station, the mayor has asked you to choose a suitable position (some integer point) for building it. You should choose the best position for the police station, so that you could minimize the total time of your criminal catching mission. Your mission of catching the criminals will operate only from this station. </p><p>The new station will have only <span class="tex-font-style-bf">one</span> patrol car. You will go to the criminals by this car, carry them on the car, bring them back to the police station and put them in prison. The patrol car can carry at most <span class="tex-span"><i>m</i></span> criminals at a time. Note that, the criminals don't know about your mission. So, they will stay where they are instead of running away.</p><p>Your task is to find the position for the police station, so that total distance you need to cover to catch all the criminals will be minimum possible. Note that, you also can built the police station on the positions where one or more criminals already exist. In such a case all these criminals are arrested instantly.</p></div><div class="input-specification"><p>The first line of the input will have two integers <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> and <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> separated by spaces. The next line will contain <span class="tex-span"><i>n</i></span> integers separated by spaces. The <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> integer is the position of the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> criminal on the <span class="tex-span"><i>x</i></span>-axis. Absolute value of positions will not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. If a criminal has position <span class="tex-span"><i>x</i></span>, he/she is located in the point <span class="tex-span">(<i>x</i>, 0)</span> of the plane. </p><p>The positions of the criminals will be given in non-decreasing order. Note, that there can be more than one criminal standing at some point of the plane.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input/output could be very large, don't use slow input/output techniques in your language. For example, do not use input/output streams (cin, cout) in C++.</p></div><div class="output-specification"><p>Print a single integer, that means the minimum possible distance you need to cover to catch all the criminals.</p></div>

## Input

<p>The first line of the input will have two integers <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>)</span> and <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup>)</span> separated by spaces. The next line will contain <span class="tex-span"><i>n</i></span> integers separated by spaces. The <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> integer is the position of the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> criminal on the <span class="tex-span"><i>x</i></span>-axis. Absolute value of positions will not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>. If a criminal has position <span class="tex-span"><i>x</i></span>, he/she is located in the point <span class="tex-span">(<i>x</i>, 0)</span> of the plane. </p><p>The positions of the criminals will be given in non-decreasing order. Note, that there can be more than one criminal standing at some point of the plane.</p><p><span class="tex-font-style-bf">Note</span>: since the size of the input/output could be very large, don't use slow input/output techniques in your language. For example, do not use input/output streams (cin, cout) in C++.</p>

## Output

<p>Print a single integer, that means the minimum possible distance you need to cover to catch all the criminals.</p>





```input1
3 6
1 2 3

```




```input2
5 5
-7 -6 -3 -1 1

```




```input3
1 369
0

```




```input4
11 2
-375 -108 1336 1453 1598 1892 2804 3732 4291 4588 4822

```




```output1
4

```




```output2
16

```




```output3
0

```




```output4
18716

```


