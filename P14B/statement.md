## Description

<div><p>Among other things, Bob is keen on photography. Especially he likes to take pictures of sportsmen. That was the reason why he placed himself in position <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span> of a long straight racetrack and got ready to take pictures. But the problem was that not all the runners passed him. The total amount of sportsmen, training at that racetrack, equals <span class="tex-span"><i>n</i></span>. And each of them regularly runs distances within a particular segment of the racetrack, which is the same for each sportsman. For example, the first sportsman runs from position <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> to position <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, the second — from <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span></p><p>What is the minimum distance that Bob should move to have a chance to take pictures of each sportsman? Bob can take a picture of a sportsman, if he stands within the segment that this sportsman covers on the racetrack.</p></div><div class="input-specification"><p>The first line of the input file contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>; <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">0</sub> ≤ 1000</span>). The following <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p></div><div class="output-specification"><p>Output the required minimum distance in the same units as the positions on the racetrack. If there is no such a position, output -1.</p></div>

## Input

<p>The first line of the input file contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index">0</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>; <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index">0</sub> ≤ 1000</span>). The following <span class="tex-span"><i>n</i></span> lines contain pairs of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>).</p>

## Output

<p>Output the required minimum distance in the same units as the positions on the racetrack. If there is no such a position, output -1.</p>





```input1
3 3
0 7
14 2
4 6

```




```output1
1

```


