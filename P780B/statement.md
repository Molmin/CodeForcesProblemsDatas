## Description

<div><p>The main road in Bytecity is a straight line from south to north. Conveniently, there are coordinates measured in meters from the southernmost building in north direction.</p><p>At some points on the road there are <span class="tex-span"><i>n</i></span> friends, and <span class="tex-span"><i>i</i></span>-th of them is standing at the point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> meters and can move with any speed no greater than <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> meters per second in any of the two directions along the road: south or north.</p><p>You are to compute the minimum time needed to gather all the <span class="tex-span"><i>n</i></span> friends at some point on the road. Note that the point they meet at doesn't need to have integer coordinate. </p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 60 000</span>)&nbsp;— the number of friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the current coordinates of the friends, in meters.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the maximum speeds of the friends, in meters per second.</p></div><div class="output-specification"><p>Print the minimum time (in seconds) needed for all the <span class="tex-span"><i>n</i></span> friends to meet at some point on the road. </p><p>Your answer will be considered correct, if its absolute or relative error isn't greater than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Formally, let your answer be <span class="tex-span"><i>a</i></span>, while jury's answer be <span class="tex-span"><i>b</i></span>. Your answer will be considered correct if <img align="middle" class="tex-formula" src="file://clvy2if5.png" style="max-width: 100.0%;max-height: 100.0%;"> holds.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 60 000</span>)&nbsp;— the number of friends.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the current coordinates of the friends, in meters.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the maximum speeds of the friends, in meters per second.</p>

## Output

<p>Print the minimum time (in seconds) needed for all the <span class="tex-span"><i>n</i></span> friends to meet at some point on the road. </p><p>Your answer will be considered correct, if its absolute or relative error isn't greater than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. Formally, let your answer be <span class="tex-span"><i>a</i></span>, while jury's answer be <span class="tex-span"><i>b</i></span>. Your answer will be considered correct if <img align="middle" class="tex-formula" src="file://clvy2if5.png" style="max-width: 100.0%;max-height: 100.0%;"> holds.</p>





```input1
3
7 1 3
1 2 1

```




```input2
4
5 10 3 2
2 3 2 4

```




```output1
2.000000000000

```




```output2
1.400000000000

```



## Note

<p>In the first sample, all friends can gather at the point <span class="tex-span">5</span> within <span class="tex-span">2</span> seconds. In order to achieve this, the first friend should go south all the time at his maximum speed, while the second and the third friends should go north at their maximum speeds.</p>
