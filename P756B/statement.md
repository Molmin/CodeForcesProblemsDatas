## Description

<div><p>A new innovative ticketing systems for public transport is introduced in Bytesburg. Now there is a single travel card for all transport. To make a trip a passenger scan his card and then he is charged according to the fare.</p><p>The fare is constructed in the following manner. There are three types of tickets: </p><ol> <li> a ticket for one trip costs <span class="tex-span">20</span> byteland rubles, </li><li> a ticket for <span class="tex-span">90</span> minutes costs <span class="tex-span">50</span> byteland rubles, </li><li> a ticket for one day (<span class="tex-span">1440</span> minutes) costs <span class="tex-span">120</span> byteland rubles. </li></ol><p>Note that a ticket for <span class="tex-span"><i>x</i></span> minutes activated at time <span class="tex-span"><i>t</i></span> can be used for trips started in time range from <span class="tex-span"><i>t</i></span> to <span class="tex-span"><i>t</i> + <i>x</i> - 1</span>, inclusive. Assume that all trips take exactly one minute.</p><p>To simplify the choice for the passenger, the system automatically chooses the optimal tickets. After each trip starts, the system analyses all the previous trips and the current trip and chooses a set of tickets for these trips with a minimum total cost. Let the minimum total cost of tickets to cover all trips from the first to the current is <span class="tex-span"><i>a</i></span>, and the total sum charged before is <span class="tex-span"><i>b</i></span>. Then the system charges the passenger the sum <span class="tex-span"><i>a</i> - <i>b</i></span>.</p><p>You have to write a program that, for given trips made by a passenger, calculates the sum the passenger is charged after each trip.</p></div><div class="input-specification"><p>The first line of input contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of trips made by passenger.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains the time of trip <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), measured in minutes from the time of starting the system. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are different, given in ascending order, i.&nbsp;e. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> + 1</sub> &gt; <i>t</i><sub class="lower-index"><i>i</i></sub></span> holds for all <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> integers. For each trip, print the sum the passenger is charged after it.</p></div>

## Input

<p>The first line of input contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of trips made by passenger.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains the time of trip <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), measured in minutes from the time of starting the system. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are different, given in ascending order, i.&nbsp;e. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> + 1</sub> &gt; <i>t</i><sub class="lower-index"><i>i</i></sub></span> holds for all <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> integers. For each trip, print the sum the passenger is charged after it.</p>





```input1
3
10
20
30

```




```input2
10
13
45
46
60
103
115
126
150
256
516

```




```output1
20
20
10

```




```output2
20
20
10
0
20
0
0
20
20
10

```



## Note

<p>In the first example, the system works as follows: for the first and second trips it is cheaper to pay for two one-trip tickets, so each time <span class="tex-span">20</span> rubles is charged, after the third trip the system understands that it would be cheaper to buy a ticket for <span class="tex-span">90</span> minutes. This ticket costs <span class="tex-span">50</span> rubles, and the passenger had already paid <span class="tex-span">40</span> rubles, so it is necessary to charge <span class="tex-span">10</span> rubles only.</p>
