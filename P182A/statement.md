## Description

<div><p>Vasya lagged behind at the University and got to the battlefield. Just joking! He's simply playing some computer game. The field is a flat platform with <span class="tex-span"><i>n</i></span> trenches dug on it. The trenches are segments on a plane parallel to the coordinate axes. No two trenches intersect.</p><p>There is a huge enemy laser far away from Vasya. The laser charges for <span class="tex-span"><i>a</i></span> seconds, and then shoots continuously for <span class="tex-span"><i>b</i></span> seconds. Then, it charges for <span class="tex-span"><i>a</i></span> seconds again. Then it shoots continuously for <span class="tex-span"><i>b</i></span> seconds again and so on. Vasya knows numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. He also knows that while the laser is shooting, Vasya must be in the trench, but while the laser is charging, Vasya can safely move around the field. The main thing is to have time to hide in the trench before the shot. If Vasya reaches the trench exactly at the moment when the laser starts shooting, we believe that Vasya managed to hide. Coincidentally, <span class="tex-font-style-bf">the length</span> of any trench in meters numerically <span class="tex-font-style-bf">does not exceed</span> <span class="tex-span"><i>b</i></span>.</p><p>Initially, Vasya is at point <span class="tex-span"><i>A</i></span>. He needs to get to point <span class="tex-span"><i>B</i></span>. Vasya moves at speed 1 meter per second in either direction. You can get in or out of the trench at any its point. Getting in or out of the trench takes no time. It is also possible to move in the trench, without leaving it.</p><p>What is the minimum time Vasya needs to get from point <span class="tex-span"><i>A</i></span> to point <span class="tex-span"><i>B</i></span>, if at the initial time the laser has just started charging? If Vasya cannot get from point <span class="tex-span"><i>A</i></span> to point <span class="tex-span"><i>B</i></span>, print -1. If Vasya reaches point <span class="tex-span"><i>B</i></span> at the moment when the laser begins to shoot, it is believed that Vasya managed to reach point <span class="tex-span"><i>B</i></span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers: <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ 1000)</span>, — the duration of charging and the duration of shooting, in seconds.</p><p>The second line contains four space-separated integers: <span class="tex-span"><i>A</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>y</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">4</sup> ≤ <i>A</i><sub class="lower-index"><i>x</i></sub>, <i>A</i><sub class="lower-index"><i>y</i></sub>, <i>B</i><sub class="lower-index"><i>x</i></sub>, <i>B</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the coordinates of points <span class="tex-span"><i>А</i></span> and <span class="tex-span"><i>B</i></span>. It is guaranteed that points <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> do not belong to any trench.</p><p>The third line contains a single integer: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>, — the number of trenches. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains four space-separated integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span">( - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the coordinates of ends of the corresponding trench.</p><p>All coordinates are given in meters. It is guaranteed that for any trench either <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>x</i><sub class="lower-index">2</sub></span>, or <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">2</sub></span>. No two trenches intersect. The length of any trench in meters doesn't exceed <span class="tex-span"><i>b</i></span> numerically.</p></div><div class="output-specification"><p>If Vasya can get from point <span class="tex-span"><i>A</i></span> to point <span class="tex-span"><i>B</i></span>, print the minimum time he will need for it. Otherwise, print number -1.</p><p>The answer will be considered correct if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span></p></div>

## Input

<p>The first line contains two space-separated integers: <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ 1000)</span>, — the duration of charging and the duration of shooting, in seconds.</p><p>The second line contains four space-separated integers: <span class="tex-span"><i>A</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>A</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>B</i><sub class="lower-index"><i>y</i></sub></span> <span class="tex-span">( - 10<sup class="upper-index">4</sup> ≤ <i>A</i><sub class="lower-index"><i>x</i></sub>, <i>A</i><sub class="lower-index"><i>y</i></sub>, <i>B</i><sub class="lower-index"><i>x</i></sub>, <i>B</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the coordinates of points <span class="tex-span"><i>А</i></span> and <span class="tex-span"><i>B</i></span>. It is guaranteed that points <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> do not belong to any trench.</p><p>The third line contains a single integer: <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000)</span>, — the number of trenches. </p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains four space-separated integers: <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span> <span class="tex-span">( - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span> — the coordinates of ends of the corresponding trench.</p><p>All coordinates are given in meters. It is guaranteed that for any trench either <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>x</i><sub class="lower-index">2</sub></span>, or <span class="tex-span"><i>y</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">2</sub></span>. No two trenches intersect. The length of any trench in meters doesn't exceed <span class="tex-span"><i>b</i></span> numerically.</p>

## Output

<p>If Vasya can get from point <span class="tex-span"><i>A</i></span> to point <span class="tex-span"><i>B</i></span>, print the minimum time he will need for it. Otherwise, print number -1.</p><p>The answer will be considered correct if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span></p>





```input1
2 4
0 5 6 5
3
0 0 0 4
1 1 4 1
6 0 6 4

```




```input2
5 10
0 0 10 10
1
5 0 5 9

```




```output1
19.0000000000

```




```output2
-1

```


