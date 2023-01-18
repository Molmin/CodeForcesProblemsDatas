## Description

<div><p>Vasya is going to the Olympics in the city Ntown by train. The boy wants to read the textbook to prepare for the Olympics. He counted that he needed <span class="tex-span"><i>k</i></span> hours for this. He also found that the light in the train changes every hour. The light is measured on a scale from 0 to 100, where 0 is very dark, and 100 is very light.</p><p>Vasya has a train lighting schedule for all <span class="tex-span"><i>n</i></span> hours of the trip — <span class="tex-span"><i>n</i></span> numbers from 0 to 100 each (the light level in the first hour, the second hour and so on). During each of those hours he will either read the whole time, or not read at all. He wants to choose <span class="tex-span"><i>k</i></span> hours to read a book, not necessarily consecutive, so that the minimum level of light among the selected hours were maximum. Vasya is very excited before the upcoming contest, help him choose reading hours.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of hours on the train and the number of hours to read, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the light level at the <span class="tex-span"><i>i</i></span>-th hour.</p></div><div class="output-specification"><p>In the first output line print the minimum light level Vasya will read at. In the second line print <span class="tex-span"><i>k</i></span> distinct space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span>, — the indexes of hours Vasya will read at (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). The hours are indexed starting from 1. If there are multiple optimal solutions, print any of them. Print the numbers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in an arbitrary order.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000, 1 ≤ <i>k</i> ≤ <i>n</i></span>) — the number of hours on the train and the number of hours to read, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the light level at the <span class="tex-span"><i>i</i></span>-th hour.</p>

## Output

<p>In the first output line print the minimum light level Vasya will read at. In the second line print <span class="tex-span"><i>k</i></span> distinct space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span>, — the indexes of hours Vasya will read at (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). The hours are indexed starting from 1. If there are multiple optimal solutions, print any of them. Print the numbers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> in an arbitrary order.</p>





```input1
5 3
20 10 30 40 10

```




```input2
6 5
90 20 35 40 60 100

```




```output1
20
1 3 4 

```




```output2
35
1 3 4 5 6 

```



## Note

<p>In the first sample Vasya should read at the first hour (light <span class="tex-span">20</span>), third hour (light <span class="tex-span">30</span>) and at the fourth hour (light <span class="tex-span">40</span>). The minimum light Vasya will have to read at is <span class="tex-span">20</span>.</p>
