## Description

<div><p>A system of <span class="tex-span"><i>n</i></span> vessels with water is given. Several pairs of vessels are connected by tubes with transfusion mechanisms. One may transfer an integer amount of liters of water between two vessels connected by such tube (tube works in both directions). There might be multiple tubes between two vessels. Total number of tubes equals <span class="tex-span"><i>e</i></span>. Volume of each vessel equals <span class="tex-span"><i>v</i></span> liters. Of course, the amount of the water in any vessel cannot exceed <span class="tex-span"><i>v</i></span> liters in the process of transfusions.</p><p>Given the initial amounts <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of water in the vessels and the desired amounts <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> find a sequence of transfusions that deals with the task. Total number of transfusions must not exceed <span class="tex-span">2·<i>n</i><sup class="upper-index">2</sup></span>.</p></div><div class="input-specification"><p>First line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>e</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>e</i> ≤ 50000</span>).</p><p>Next two lines contain <span class="tex-span"><i>n</i></span> integers each: initial <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and the desired amounts <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of water in corresponding vessels (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>v</i></span>).</p><p>Next <span class="tex-span"><i>e</i></span> lines describe one tube each in the format <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>) for a tube between vessels number <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. There might be multiple tubes between two vessels. You may assume that vessels are numbered from 1 to <span class="tex-span"><i>n</i></span> in some way.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes), if such sequence of transfusions does not exist.</p><p>Otherwise print any suitable sequence in the following format. On the first line print the total number of transfusions <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i></span> should not exceed <span class="tex-span">2·<i>n</i><sup class="upper-index">2</sup></span>). In the following <span class="tex-span"><i>k</i></span> lines print transfusions in the format <span class="tex-span"><i>x</i></span>&nbsp;<span class="tex-span"><i>y</i></span>&nbsp;<span class="tex-span"><i>d</i></span> (transfusion of <span class="tex-span"><i>d</i></span> liters from the vessel number <span class="tex-span"><i>x</i></span> to the vessel number <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> must be distinct). For all transfusions <span class="tex-span"><i>d</i></span> must be a non-negative integer.</p></div>

## Input

<p>First line of the input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>v</i></span>, <span class="tex-span"><i>e</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 300</span>, <span class="tex-span">1 ≤ <i>v</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>e</i> ≤ 50000</span>).</p><p>Next two lines contain <span class="tex-span"><i>n</i></span> integers each: initial <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and the desired amounts <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of water in corresponding vessels (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>v</i></span>).</p><p>Next <span class="tex-span"><i>e</i></span> lines describe one tube each in the format <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>, <i>x</i> ≠ <i>y</i></span>) for a tube between vessels number <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. There might be multiple tubes between two vessels. You may assume that vessels are numbered from 1 to <span class="tex-span"><i>n</i></span> in some way.</p>

## Output

<p>Print "<span class="tex-font-style-tt">NO</span>" (without quotes), if such sequence of transfusions does not exist.</p><p>Otherwise print any suitable sequence in the following format. On the first line print the total number of transfusions <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i></span> should not exceed <span class="tex-span">2·<i>n</i><sup class="upper-index">2</sup></span>). In the following <span class="tex-span"><i>k</i></span> lines print transfusions in the format <span class="tex-span"><i>x</i></span>&nbsp;<span class="tex-span"><i>y</i></span>&nbsp;<span class="tex-span"><i>d</i></span> (transfusion of <span class="tex-span"><i>d</i></span> liters from the vessel number <span class="tex-span"><i>x</i></span> to the vessel number <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> must be distinct). For all transfusions <span class="tex-span"><i>d</i></span> must be a non-negative integer.</p>





```input1
2 10 1
1 9
5 5
1 2

```




```input2
2 10 0
5 2
4 2

```




```input3
2 10 0
4 2
4 2

```




```output1
1
2 1 4

```




```output2
NO

```




```output3
0

```


