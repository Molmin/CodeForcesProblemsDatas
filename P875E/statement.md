## Description

<div><p>Petya and Vasya got employed as couriers. During the working day they are to deliver packages to <span class="tex-span"><i>n</i></span> different points on the line. According to the company's internal rules, the delivery of packages must be carried out strictly in a certain order. Initially, Petya is at the point with the coordinate <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, Vasya is at the point with the coordinate <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>, and the clients are at the points <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> in the order of the required visit.</p><p>The guys agree in advance who of them will deliver the package to which of the customers, and then they act as follows. When the package for the <span class="tex-span"><i>i</i></span>-th client is delivered, the one who delivers the package to the <span class="tex-span">(<i>i</i> + 1)</span>-st client is sent to the path (it can be the same person who went to the point <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, or the other). The friend who is not busy in delivering the current package, is standing still.</p><p>To communicate with each other, the guys have got walkie-talkies. The walkie-talkies work rather poorly at great distances, so Petya and Vasya want to distribute the orders so that the maximum distance between them during the day is as low as possible. Help Petya and Vasya to minimize the maximum distance between them, observing all delivery rules. </p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— number of points of delivery and starting positions of Petya and Vasya.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— customers coordinates (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), in the order to make a delivery. </p><p>It is guaranteed, that among the numbers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> there are no two equal.</p></div><div class="output-specification"><p>Output the only integer, minimum possible maximal distance between couriers during delivery.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">0 ≤ <i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— number of points of delivery and starting positions of Petya and Vasya.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;— customers coordinates (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), in the order to make a delivery. </p><p>It is guaranteed, that among the numbers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>x</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> there are no two equal.</p>

## Output

<p>Output the only integer, minimum possible maximal distance between couriers during delivery.</p>





```input1
2 0 10
5 6

```




```input2
3 2 1
3 4 5

```




```input3
1 4 5
2

```




```output1
10

```




```output2
1

```




```output3
2

```



## Note

<p>In the first test case the initial distance between the couriers is <span class="tex-span">10</span>. This value will be the answer, for example, Petya can perform both deliveries, and Vasya will remain at the starting point.</p><p>In the second test case you can optimally act, for example, like this: Vasya delivers the package to the first customer, Petya to the second and, finally, Vasya delivers the package to the third client. With this order of delivery, the distance between the couriers will never exceed <span class="tex-span">1</span>.</p><p>In the third test case only two variants are possible: if the delivery of a single package is carried out by Petya, the maximum distance between them will be <span class="tex-span">5 - 2 = 3</span>. If Vasya will deliver the package, the maximum distance is <span class="tex-span">4 - 2 = 2</span>. The latter method is optimal.</p>
