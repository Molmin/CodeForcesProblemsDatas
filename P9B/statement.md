## Description

<div><p>And again a misfortune fell on Poor Student. He is being late for an exam.</p><p>Having rushed to a bus stop that is in point <span class="tex-span">(0, 0)</span>, he got on a minibus and they drove along a straight line, parallel to axis <span class="tex-span"><i>OX</i></span>, in the direction of increasing <span class="tex-span"><i>x</i></span>.</p><p>Poor Student knows the following: </p><ul> <li> during one run the minibus makes <span class="tex-span"><i>n</i></span> stops, the <span class="tex-span"><i>i</i></span>-th stop is in point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, 0)</span> </li><li> coordinates of all the stops are different </li><li> the minibus drives at a constant speed, equal to <span class="tex-span"><i>v</i><sub class="lower-index"><i>b</i></sub></span> </li><li> it can be assumed the passengers get on and off the minibus at a bus stop momentarily </li><li> Student can get off the minibus only at a bus stop </li><li> Student will have to get off the minibus at a terminal stop, if he does not get off earlier </li><li> the University, where the exam will be held, is in point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>u</i></sub>, <i>y</i><sub class="lower-index"><i>u</i></sub>)</span> </li><li> Student can run from a bus stop to the University at a constant speed <span class="tex-span"><i>v</i><sub class="lower-index"><i>s</i></sub></span> as long as needed </li><li> a distance between two points can be calculated according to the following formula: <img align="middle" class="tex-formula" src="file://GBAVchit.png" style="max-width: 100.0%;max-height: 100.0%;"> </li><li> Student is already on the minibus, so, he cannot get off at the first bus stop </li></ul><p>Poor Student wants to get to the University as soon as possible. Help him to choose the bus stop, where he should get off. If such bus stops are multiple, choose the bus stop closest to the University.</p></div><div class="input-specification"><p>The first line contains three integer numbers: <span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>b</i></sub>, <i>v</i><sub class="lower-index"><i>s</i></sub> ≤ 1000</span>. The second line contains <span class="tex-span"><i>n</i></span> non-negative integers in ascending order: coordinates <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> of the bus stop with index <span class="tex-span"><i>i</i></span>. It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> equals to zero, and <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">5</sup></span>. The third line contains the coordinates of the University, integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>u</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>u</i></sub></span>, not exceeding <span class="tex-span">10<sup class="upper-index">5</sup></span> in absolute value. </p></div><div class="output-specification"><p>In the only line output the answer to the problem — index of the optimum bus stop.</p></div>

## Input

<p>The first line contains three integer numbers: <span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>b</i></sub>, <i>v</i><sub class="lower-index"><i>s</i></sub> ≤ 1000</span>. The second line contains <span class="tex-span"><i>n</i></span> non-negative integers in ascending order: coordinates <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> of the bus stop with index <span class="tex-span"><i>i</i></span>. It is guaranteed that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> equals to zero, and <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">5</sup></span>. The third line contains the coordinates of the University, integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>u</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>u</i></sub></span>, not exceeding <span class="tex-span">10<sup class="upper-index">5</sup></span> in absolute value. </p>

## Output

<p>In the only line output the answer to the problem — index of the optimum bus stop.</p>





```input1
4 5 2
0 2 4 6
4 1

```




```input2
2 1 1
0 100000
100000 100000

```




```output1
3
```




```output2
2
```



## Note

<p>As you know, students are a special sort of people, and minibuses usually do not hurry. That's why you should not be surprised, if Student's speed is higher than the speed of the minibus.</p>
