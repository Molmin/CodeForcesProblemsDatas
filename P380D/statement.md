## Description

<div><p>The cinema theater hall in Sereja's city is <span class="tex-span"><i>n</i></span> seats lined up in front of one large screen. There are slots for personal possessions to the left and to the right of each seat. Any two adjacent seats have exactly one shared slot. The figure below shows the arrangement of seats and slots for <span class="tex-span"><i>n</i> = 4</span>.</p><center> <img class="tex-graphics" src="file://WCViqSis.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Today it's the premiere of a movie called "Dry Hard". The tickets for all the seats have been sold. There is a very strict controller at the entrance to the theater, so all <span class="tex-span"><i>n</i></span> people will come into the hall one by one. As soon as a person enters a cinema hall, he immediately (momentarily) takes his seat and occupies all empty slots to the left and to the right from him. If there are no empty slots, the man gets really upset and leaves.</p><p>People are not very constant, so it's hard to predict the order in which the viewers will enter the hall. For some seats, Sereja knows the number of the viewer (his number in the entering queue of the viewers) that will come and take this seat. For others, it can be any order. </p><p>Being a programmer and a mathematician, Sereja wonders: how many ways are there for the people to enter the hall, such that nobody gets upset? As the number can be quite large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th integer shows either the index of the person (index in the entering queue) with the ticket for the <span class="tex-span"><i>i</i></span>-th seat or a <span class="tex-span">0</span>, if his index is not known. It is guaranteed that all positive numbers in the second line are distinct.</p><p>You can assume that the index of the person who enters the cinema hall is a unique integer from 1 to <span class="tex-span"><i>n</i></span>. The person who has index 1 comes first to the hall, the person who has index 2 comes second and so on.</p></div><div class="output-specification"><p>In a single line print the remainder after dividing the answer by number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th integer shows either the index of the person (index in the entering queue) with the ticket for the <span class="tex-span"><i>i</i></span>-th seat or a <span class="tex-span">0</span>, if his index is not known. It is guaranteed that all positive numbers in the second line are distinct.</p><p>You can assume that the index of the person who enters the cinema hall is a unique integer from 1 to <span class="tex-span"><i>n</i></span>. The person who has index 1 comes first to the hall, the person who has index 2 comes second and so on.</p>

## Output

<p>In a single line print the remainder after dividing the answer by number <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
11
0 0 0 0 0 0 0 0 0 0 0

```




```input2
6
0 3 1 0 0 0

```




```output1
1024

```




```output2
3

```


