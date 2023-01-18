## Description

<div><p>A parking lot in the City consists of <span class="tex-span"><i>n</i></span> parking spaces, standing in a line. The parking spaces are numbered from 1 to <span class="tex-span"><i>n</i></span> from left to right. </p><p>When a car arrives at the lot, the operator determines an empty parking space for it. For the safety's sake the chosen place should be located as far from the already occupied places as possible. That is, the closest occupied parking space must be as far away as possible. If there are several such places, then the operator chooses the place with the minimum index from them. If all parking lot places are empty, then the car gets place number <span class="tex-span">1</span>.</p><p>We consider the distance between the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th parking spaces equal to <span class="tex-span">4·|<i>i</i> - <i>j</i>|</span> meters.</p><p>You are given the parking lot records of arriving and departing cars in the chronological order. For each record of an arriving car print the number of the parking lot that was given to this car.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of parking places and the number of records correspondingly. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the records, one per line. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2;&nbsp;1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals 1, then the corresponding record says that the car number <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> arrived at the parking lot. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals 2, then the corresponding record says that the car number <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> departed from the parking lot. </p><p>Records about arriving to the parking lot and departing from the parking lot are given chronologically. All events occurred consecutively, no two events occurred simultaneously.</p><p>It is guaranteed that all entries are correct: </p><ul> <li> each car arrived at the parking lot at most once and departed from the parking lot at most once, </li><li> there is no record of a departing car if it didn't arrive at the parking lot earlier, </li><li> there are no more than <span class="tex-span"><i>n</i></span> cars on the parking lot at any moment. </li></ul> <p>You can consider the cars arbitrarily numbered from 1 to <span class="tex-span">10<sup class="upper-index">6</sup></span>, all numbers are distinct. Initially all places in the parking lot are empty.</p></div><div class="output-specification"><p>For each entry of an arriving car print the number of its parking space. Print the numbers of the spaces in the order, in which the cars arrive to the parking lot.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup>)</span> — the number of parking places and the number of records correspondingly. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the records, one per line. The <span class="tex-span"><i>i</i></span>-th line contains numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2;&nbsp;1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals 1, then the corresponding record says that the car number <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> arrived at the parking lot. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals 2, then the corresponding record says that the car number <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> departed from the parking lot. </p><p>Records about arriving to the parking lot and departing from the parking lot are given chronologically. All events occurred consecutively, no two events occurred simultaneously.</p><p>It is guaranteed that all entries are correct: </p><ul> <li> each car arrived at the parking lot at most once and departed from the parking lot at most once, </li><li> there is no record of a departing car if it didn't arrive at the parking lot earlier, </li><li> there are no more than <span class="tex-span"><i>n</i></span> cars on the parking lot at any moment. </li></ul> <p>You can consider the cars arbitrarily numbered from 1 to <span class="tex-span">10<sup class="upper-index">6</sup></span>, all numbers are distinct. Initially all places in the parking lot are empty.</p>

## Output

<p>For each entry of an arriving car print the number of its parking space. Print the numbers of the spaces in the order, in which the cars arrive to the parking lot.</p>





```input1
7 11
1 15
1 123123
1 3
1 5
2 123123
2 15
1 21
2 3
1 6
1 7
1 8

```




```output1
1
7
4
2
7
4
1
3

```


