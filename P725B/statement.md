## Description

<div><p>A new airplane SuperPuperJet has an infinite number of rows, numbered with positive integers starting with <span class="tex-span">1</span> from cockpit to tail. There are six seats in each row, denoted with letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">f</span>'. Seats '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">c</span>' are located to the left of an aisle (if one looks in the direction of the cockpit), while seats '<span class="tex-font-style-tt">d</span>', '<span class="tex-font-style-tt">e</span>' and '<span class="tex-font-style-tt">f</span>' are located to the right. Seats '<span class="tex-font-style-tt">a</span>' and '<span class="tex-font-style-tt">f</span>' are located near the windows, while seats '<span class="tex-font-style-tt">c</span>' and '<span class="tex-font-style-tt">d</span>' are located near the aisle. </p><center> <img class="tex-graphics" height="197px" src="file://lr9XZrB8.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>&nbsp;</p><p>It's lunch time and two flight attendants have just started to serve food. They move from the first rows to the tail, always maintaining a distance of two rows from each other because of the food trolley. Thus, at the beginning the first attendant serves row <span class="tex-span">1</span> while the second attendant serves row <span class="tex-span">3</span>. When both rows are done they move one row forward: the first attendant serves row <span class="tex-span">2</span> while the second attendant serves row <span class="tex-span">4</span>. Then they move three rows forward and the first attendant serves row <span class="tex-span">5</span> while the second attendant serves row <span class="tex-span">7</span>. Then they move one row forward again and so on.</p><p>Flight attendants work with the same speed: it takes exactly <span class="tex-span">1</span> second to serve one passenger and <span class="tex-span">1</span> second to move one row forward. Each attendant first serves the passengers on the seats to the right of the aisle and then serves passengers on the seats to the left of the aisle (if one looks in the direction of the cockpit). Moreover, they always serve passengers in order from the window to the aisle. Thus, the first passenger to receive food in each row is located in seat '<span class="tex-font-style-tt">f</span>', and the last one&nbsp;— in seat '<span class="tex-font-style-tt">c</span>'. Assume that all seats are occupied.</p><p>Vasya has seat <span class="tex-span"><i>s</i></span> in row <span class="tex-span"><i>n</i></span> and wants to know how many seconds will pass before he gets his lunch.</p></div><div class="input-specification"><p>The only line of input contains a description of Vasya's seat in the format <span class="tex-span"><i>ns</i></span>, where <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>) is the index of the row and <span class="tex-span"><i>s</i></span> is the seat in this row, denoted as letter from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">f</span>'. The index of the row and the seat <span class="tex-font-style-bf">are not separated</span> by a space.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the number of seconds Vasya has to wait until he gets his lunch.</p></div>

## Input

<p>The only line of input contains a description of Vasya's seat in the format <span class="tex-span"><i>ns</i></span>, where <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup></span>) is the index of the row and <span class="tex-span"><i>s</i></span> is the seat in this row, denoted as letter from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">f</span>'. The index of the row and the seat <span class="tex-font-style-bf">are not separated</span> by a space.</p>

## Output

<p>Print one integer&nbsp;— the number of seconds Vasya has to wait until he gets his lunch.</p>





```input1
1f

```




```input2
2d

```




```input3
4a

```




```input4
5e

```




```output1
1

```




```output2
10

```




```output3
11

```




```output4
18

```



## Note

<p>In the first sample, the first flight attendant serves Vasya first, so Vasya gets his lunch after <span class="tex-span">1</span> second.</p><p>In the second sample, the flight attendants will spend <span class="tex-span">6</span> seconds to serve everyone in the rows <span class="tex-span">1</span> and <span class="tex-span">3</span>, then they will move one row forward in <span class="tex-span">1</span> second. As they first serve seats located to the right of the aisle in order from window to aisle, Vasya has to wait <span class="tex-span">3</span> more seconds. The total is <span class="tex-span">6 + 1 + 3 = 10</span>.</p>
