## Description

<div><p>The R1 company wants to hold a web search championship. There were <span class="tex-span"><i>n</i></span> computers given for the competition, each of them is connected to the Internet. The organizers believe that the data transfer speed directly affects the result. The higher the speed of the Internet is, the faster the participant will find the necessary information. Therefore, before the competition started, each computer had its maximum possible data transfer speed measured. On the <span class="tex-span"><i>i</i></span>-th computer it was <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> kilobits per second.</p><p>There will be <span class="tex-span"><i>k</i></span> participants competing in the championship, each should get a separate computer. The organizing company does not want any of the participants to have an advantage over the others, so they want to provide the same data transfer speed to each participant's computer. Also, the organizers want to create the most comfortable conditions for the participants, so the data transfer speed on the participants' computers should be as large as possible.</p><p>The network settings of the R1 company has a special option that lets you to cut the initial maximum data transfer speed of any computer to any lower speed. How should the R1 company configure the network using the described option so that at least <span class="tex-span"><i>k</i></span> of <span class="tex-span"><i>n</i></span> computers had the same data transfer speed and the data transfer speed on these computers was as large as possible?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span> — the number of computers and the number of participants, respectively. In the second line you have a space-separated sequence consisting of <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(16 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 32768)</span>; number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the maximum data transfer speed on the <span class="tex-span"><i>i</i></span>-th computer.</p></div><div class="output-specification"><p>Print a single integer — the maximum Internet speed value. It is guaranteed that the answer to the problem is always an integer.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100)</span> — the number of computers and the number of participants, respectively. In the second line you have a space-separated sequence consisting of <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(16 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 32768)</span>; number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> denotes the maximum data transfer speed on the <span class="tex-span"><i>i</i></span>-th computer.</p>

## Output

<p>Print a single integer — the maximum Internet speed value. It is guaranteed that the answer to the problem is always an integer.</p>





```input1
3 2
40 20 30

```




```input2
6 4
100 20 40 20 50 50

```




```output1
30

```




```output2
40

```



## Note

<p>In the first test case the organizers can cut the first computer's speed to <span class="tex-span">30</span> kilobits. Then two computers (the first and the third one) will have the same speed of <span class="tex-span">30</span> kilobits. They should be used as the participants' computers. This answer is optimal.</p>
