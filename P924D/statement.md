## Description

<div><p>Arkady the air traffic controller is now working with <span class="tex-span"><i>n</i></span> planes in the air. All planes move along a straight coordinate axis with Arkady's station being at point <span class="tex-span">0</span> on it. The <span class="tex-span"><i>i</i></span>-th plane, small enough to be represented by a point, currently has a coordinate of <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and is moving with speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>·<i>v</i><sub class="lower-index"><i>i</i></sub> &lt; 0</span>, i.e., all planes are moving towards the station.</p><p>Occasionally, the planes are affected by winds. With a wind of speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>wind</i></sub></span> (not necessarily positive or integral), the speed of the <span class="tex-span"><i>i</i></span>-th plane becomes <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> + <i>v</i><sub class="lower-index"><i>wind</i></sub></span>.</p><p>According to weather report, the current wind has a steady speed falling inside the range <span class="tex-span">[ - <i>w</i>, <i>w</i>]</span> (inclusive), but the exact value cannot be measured accurately since this value is rather small — smaller than the absolute value of speed of any plane.</p><p>Each plane should contact Arkady at the exact moment it passes above his station. And you are to help Arkady count the number of pairs of planes <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) there are such that there is a possible value of wind speed, under which planes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> contact Arkady at the same moment. This value needn't be the same across different pairs.</p><p>The wind speed is the same for all planes. You may assume that the wind has a steady speed and lasts arbitrarily long.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>w</i> &lt; 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of planes and the maximum wind speed.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>w</i> + 1 ≤ |<i>v</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>·<i>v</i><sub class="lower-index"><i>i</i></sub> &lt; 0</span>)&nbsp;— the initial position and speed of the <span class="tex-span"><i>i</i></span>-th plane.</p><p>Planes are pairwise distinct, that is, no pair of <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) exists such that both <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> = <i>v</i><sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of unordered pairs of planes that can contact Arkady at the same moment.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>w</i> &lt; 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of planes and the maximum wind speed.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>x</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>w</i> + 1 ≤ |<i>v</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>·<i>v</i><sub class="lower-index"><i>i</i></sub> &lt; 0</span>)&nbsp;— the initial position and speed of the <span class="tex-span"><i>i</i></span>-th plane.</p><p>Planes are pairwise distinct, that is, no pair of <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>) exists such that both <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> = <i>x</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> = <i>v</i><sub class="lower-index"><i>j</i></sub></span>.</p>

## Output

<p>Output a single integer&nbsp;— the number of unordered pairs of planes that can contact Arkady at the same moment.</p>





```input1
5 1
-3 2
-3 3
-1 2
1 -3
3 -5

```




```input2
6 1
-3 2
-2 2
-1 2
1 -2
2 -2
3 -2

```




```output1
3

```




```output2
9

```



## Note

<p>In the first example, the following <span class="tex-span">3</span> pairs of planes satisfy the requirements: </p><ul> <li> <span class="tex-font-style-bf"><span class="tex-span">(2, 5)</span></span> passes the station at time <span class="tex-span">3 / 4</span> with <span class="tex-span"><i>v</i><sub class="lower-index"><i>wind</i></sub> = 1</span>; </li><li> <span class="tex-font-style-bf"><span class="tex-span">(3, 4)</span></span> passes the station at time <span class="tex-span">2 / 5</span> with <span class="tex-span"><i>v</i><sub class="lower-index"><i>wind</i></sub> = 1 / 2</span>; </li><li> <span class="tex-font-style-bf"><span class="tex-span">(3, 5)</span></span> passes the station at time <span class="tex-span">4 / 7</span> with <span class="tex-span"><i>v</i><sub class="lower-index"><i>wind</i></sub> =  - 1 / 4</span>. </li></ul><p>In the second example, each of the <span class="tex-span">3</span> planes with negative coordinates can form a valid pair with each of the other <span class="tex-span">3</span>, totaling <span class="tex-span">9</span> pairs.</p>
