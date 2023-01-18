## Description

<div><p>The project of a data center of a Big Software Company consists of <span class="tex-span"><i>n</i></span> computers connected by <span class="tex-span"><i>m</i></span> cables. Simply speaking, each computer can be considered as a box with multiple cables going out of the box. Very Important Information is transmitted along each cable in one of the two directions. As the data center plan is not yet approved, it wasn't determined yet in which direction information will go along each cable. The cables are put so that each computer is connected with each one, perhaps through some other computers.</p><p>The person in charge of the cleaning the data center will be Claudia Ivanova, the janitor. She loves to tie cables into bundles using cable ties. For some reasons, she groups the cables sticking out of a computer into groups of two, and if it isn't possible, then she gets furious and attacks the computer with the water from the bucket.</p><p>It should also be noted that due to the specific physical characteristics of the Very Important Information, it is strictly forbidden to connect in one bundle two cables where information flows in different directions.</p><p>The management of the data center wants to determine how to send information along each cable so that Claudia Ivanova is able to group all the cables coming out of each computer into groups of two, observing the condition above. Since it may not be possible with the existing connections plan, you are allowed to add the minimum possible number of cables to the scheme, and then you need to determine the direction of the information flow for each cable (yes, sometimes data centers are designed based on the janitors' convenience...)</p></div><div class="input-specification"><p>The first line contains two numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>) — the number of computers and the number of the already present cables, respectively.</p><p>Each of the next lines contains two numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the indices of the computers connected by the <span class="tex-span"><i>i</i></span>-th cable. The data centers often have a very complex structure, so a pair of computers may have more than one pair of cables between them and some cables may connect a computer with itself.</p></div><div class="output-specification"><p>In the first line print a single number <span class="tex-span"><i>p</i></span> (<span class="tex-span"><i>p</i> ≥ <i>m</i></span>) — the minimum number of cables in the final scheme.</p><p>In each of the next <span class="tex-span"><i>p</i></span> lines print a pair of numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing another cable. Such entry means that information will go along a certain cable in direction from <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Among the cables you printed there should be all the cables presented in the original plan in some of two possible directions. It is guaranteed that there is a solution where <span class="tex-span"><i>p</i></span> doesn't exceed <span class="tex-span">500 000</span>.</p><p>If there are several posible solutions with minimum possible value of <span class="tex-span"><i>p</i></span>, print any of them.</p></div>

## Input

<p>The first line contains two numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>) — the number of computers and the number of the already present cables, respectively.</p><p>Each of the next lines contains two numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the indices of the computers connected by the <span class="tex-span"><i>i</i></span>-th cable. The data centers often have a very complex structure, so a pair of computers may have more than one pair of cables between them and some cables may connect a computer with itself.</p>

## Output

<p>In the first line print a single number <span class="tex-span"><i>p</i></span> (<span class="tex-span"><i>p</i> ≥ <i>m</i></span>) — the minimum number of cables in the final scheme.</p><p>In each of the next <span class="tex-span"><i>p</i></span> lines print a pair of numbers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing another cable. Such entry means that information will go along a certain cable in direction from <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Among the cables you printed there should be all the cables presented in the original plan in some of two possible directions. It is guaranteed that there is a solution where <span class="tex-span"><i>p</i></span> doesn't exceed <span class="tex-span">500 000</span>.</p><p>If there are several posible solutions with minimum possible value of <span class="tex-span"><i>p</i></span>, print any of them.</p>





```input1
4 6
1 2
2 3
3 4
4 1
1 3
1 3

```




```input2
3 4
1 2
2 3
1 1
3 3

```




```output1
6
1 2
3 4
1 4
3 2
1 3
1 3
```




```output2
6
2 1
2 3
1 1
3 3
3 1
1 1

```



## Note

<p>Picture for the first sample test. The tied pairs of cables are shown going out from the same point.</p><center> <img class="tex-graphics" src="file://e9WbQq0H.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Picture for the second test from the statement. The added cables are drawin in bold.</p><center> <img class="tex-graphics" src="file://lEHH2LTk.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Alternative answer for the second sample test:</p><center> <img class="tex-graphics" src="file://6fH3NEaJ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
