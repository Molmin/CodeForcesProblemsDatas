## Description

<div><p>Lolek and Bolek are about to travel abroad by plane. The local airport has a special "Choose Your Plane" offer. The offer's conditions are as follows:</p><ul> <li> it is up to a passenger to choose a plane to fly on; </li><li> if the chosen plane has <span class="tex-span"><i>x</i></span> <span class="tex-span">(<i>x</i> &gt; 0)</span> empty seats at the given moment, then the ticket for such a plane costs <span class="tex-span"><i>x</i></span> zlotys (units of Polish currency). </li></ul><p>The only ticket office of the airport already has a queue of <span class="tex-span"><i>n</i></span> passengers in front of it. Lolek and Bolek have not stood in the queue yet, but they are already wondering what is the maximum and the minimum number of zlotys the airport administration can earn if all <span class="tex-span"><i>n</i></span> passengers buy tickets according to the conditions of this offer?</p><p>The passengers buy tickets in turn, the first person in the queue goes first, then goes the second one, and so on up to <span class="tex-span"><i>n</i></span>-th person.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span> — the number of passengers in the queue and the number of planes in the airport, correspondingly. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of empty seats in the <span class="tex-span"><i>i</i></span>-th plane before the ticket office starts selling tickets.</p><p>The numbers in the lines are separated by a space. It is guaranteed that there are at least <span class="tex-span"><i>n</i></span> empty seats in total.</p></div><div class="output-specification"><p>Print two integers — the maximum and the minimum number of zlotys that the airport administration can earn, correspondingly.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 1000)</span> — the number of passengers in the queue and the number of planes in the airport, correspondingly. The next line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> stands for the number of empty seats in the <span class="tex-span"><i>i</i></span>-th plane before the ticket office starts selling tickets.</p><p>The numbers in the lines are separated by a space. It is guaranteed that there are at least <span class="tex-span"><i>n</i></span> empty seats in total.</p>

## Output

<p>Print two integers — the maximum and the minimum number of zlotys that the airport administration can earn, correspondingly.</p>





```input1
4 3
2 1 1

```




```input2
4 3
2 2 2

```




```output1
5 5

```




```output2
7 6

```



## Note

<p>In the first test sample the number of passengers is equal to the number of empty seats, so regardless of the way the planes are chosen, the administration will earn the same sum.</p><p>In the second sample the sum is maximized if the 1-st person in the queue buys a ticket to the 1-st plane, the 2-nd person — to the 2-nd plane, the 3-rd person — to the 3-rd plane, the 4-th person — to the 1-st plane. The sum is minimized if the 1-st person in the queue buys a ticket to the 1-st plane, the 2-nd person — to the 1-st plane, the 3-rd person — to the 2-nd plane, the 4-th person — to the 2-nd plane.</p>
