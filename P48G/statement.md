## Description

<div><p>In a far away galaxy there are <span class="tex-span"><i>n</i></span> inhabited planets numbered with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. One day the presidents of all the <span class="tex-span"><i>n</i></span> planets independently from each other came up with an idea of creating the Galaxy Union. Now they need to share this wonderful idea with their galaxymates, that’s why each president is busy working out a project of negotiating with the other presidents.</p><p>For negotiations between some pairs of the planets there are bidirectional communication channels, each of which is characterized with "dial duration" <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> which, as a rule, takes several hours and exceeds the call duration greatly. Overall the galaxy has <span class="tex-span"><i>n</i></span> communication channels and they unite all the planets into a uniform network. That means that it is possible to phone to any planet <span class="tex-span"><i>v</i></span> from any planet <span class="tex-span"><i>u</i></span>, perhaps, using some transitional planets <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>v</i><sub class="lower-index"><i>m</i></sub></span> via the existing channels between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>v</i><sub class="lower-index"><i>m</i> - 1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>m</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>m</i></sub></span> and <span class="tex-span"><i>v</i></span>. At that the dial duration from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> will be equal to the sum of dial durations of the used channels.</p><p>So, every president has to talk one by one to the presidents of all the rest <span class="tex-span"><i>n</i> - 1</span> planets. At that the negotiations take place strictly consecutively, and until the negotiations with a planet stop, the dial to another one does not begin. As the matter is urgent, from the different ways to call the needed planet every time the quickest one is chosen. Little time is needed to assure another president on the importance of the Galaxy Union, that’s why the duration of the negotiations with each planet can be considered equal to the dial duration time for those planets. As the presidents know nothing about each other’s plans, they do not take into consideration the possibility that, for example, the sought president may call himself or already know about the founding of the Galaxy Union from other sources.</p><p>The governments of all the <span class="tex-span"><i>n</i></span> planets asked you to work out the negotiation plans. First you are to find out for every president how much time his supposed negotiations will take.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 200000</span>) which represents the number of planets in the Galaxy and the number of communication channels equal to it. The next <span class="tex-span"><i>n</i></span> lines contain three integers each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>) that represent the numbers of planet joined by a communication channel and its "dial duration". There can be no more than one communication channel between a pair of planets. </p></div><div class="output-specification"><p>In the first line output <span class="tex-span"><i>n</i></span> integers — the durations of the supposed negotiations for each president. Separate the numbers by spaces.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 200000</span>) which represents the number of planets in the Galaxy and the number of communication channels equal to it. The next <span class="tex-span"><i>n</i></span> lines contain three integers each <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>) that represent the numbers of planet joined by a communication channel and its "dial duration". There can be no more than one communication channel between a pair of planets. </p>

## Output

<p>In the first line output <span class="tex-span"><i>n</i></span> integers — the durations of the supposed negotiations for each president. Separate the numbers by spaces.</p>





```input1
3
1 2 3
2 3 2
1 3 1

```




```input2
3
1 2 3
2 3 2
1 3 5

```




```input3
4
1 2 3
2 3 2
3 4 1
4 1 4

```




```output1
4 5 3

```




```output2
8 5 7

```




```output3
12 8 8 8

```


