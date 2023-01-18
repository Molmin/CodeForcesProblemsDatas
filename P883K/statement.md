## Description

<div><p>Mayor of city S just hates trees and lawns. They take so much space and there could be a road on the place they occupy!</p><p>The Mayor thinks that one of the main city streets could be considerably widened on account of lawn nobody needs anyway. Moreover, that might help reduce the car jams which happen from time to time on the street.</p><p>The street is split into <span class="tex-span"><i>n</i></span> equal length parts from left to right, the <span class="tex-span"><i>i</i></span>-th part is characterized by two integers: width of road <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and width of lawn <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span>.</p><center> <img class="tex-graphics" src="file://vfQfQn3Z.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For each of <span class="tex-span"><i>n</i></span> parts the Mayor should decide the size of lawn to demolish. For the <span class="tex-span"><i>i</i></span>-th part he can reduce lawn width by integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>g</i><sub class="lower-index"><i>i</i></sub></span>). After it new road width of the <span class="tex-span"><i>i</i></span>-th part will be equal to <span class="tex-span"><i>s</i>'<sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>i</i></sub> + <i>x</i><sub class="lower-index"><i>i</i></sub></span> and new lawn width will be equal to <span class="tex-span"><i>g</i>'<sub class="lower-index"><i>i</i></sub> = <i>g</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>On the one hand, the Mayor wants to demolish as much lawn as possible (and replace it with road). On the other hand, he does not want to create a rapid widening or narrowing of the road, which would lead to car accidents. To avoid that, the Mayor decided that width of the road for consecutive parts should differ by at most <span class="tex-span">1</span>, i.e. for each <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>) the inequation <span class="tex-span">|<i>s</i>'<sub class="lower-index"><i>i</i> + 1</sub> - <i>s</i>'<sub class="lower-index"><i>i</i></sub>| ≤ 1</span> should hold. Initially this condition might not be true.</p><p>You need to find the the total width of lawns the Mayor will destroy according to his plan.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of parts of the street.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>g</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — current width of road and width of the lawn on the <span class="tex-span"><i>i</i></span>-th part of the street.</p></div><div class="output-specification"><p>In the first line print the total width of lawns which will be removed.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i>'<sub class="lower-index">1</sub>, <i>s</i>'<sub class="lower-index">2</sub>, ..., <i>s</i>'<sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>s</i>'<sub class="lower-index"><i>i</i></sub> ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> + <i>g</i><sub class="lower-index"><i>i</i></sub></span>) — new widths of the road starting from the first part and to the last.</p><p>If there is no solution, print the only integer <span class="tex-font-style-tt">-1</span> in the first line.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of parts of the street.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub>, <i>g</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — current width of road and width of the lawn on the <span class="tex-span"><i>i</i></span>-th part of the street.</p>

## Output

<p>In the first line print the total width of lawns which will be removed.</p><p>In the second line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i>'<sub class="lower-index">1</sub>, <i>s</i>'<sub class="lower-index">2</sub>, ..., <i>s</i>'<sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>s</i>'<sub class="lower-index"><i>i</i></sub> ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> + <i>g</i><sub class="lower-index"><i>i</i></sub></span>) — new widths of the road starting from the first part and to the last.</p><p>If there is no solution, print the only integer <span class="tex-font-style-tt">-1</span> in the first line.</p>





```input1
3
4 5
4 5
4 10

```




```input2
4
1 100
100 1
1 100
100 1

```




```input3
3
1 1
100 100
1 1

```




```output1
16
9 9 10 

```




```output2
202
101 101 101 101 

```




```output3
-1

```


