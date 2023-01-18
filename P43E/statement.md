## Description

<div><p>Today <span class="tex-span"><i>s</i></span> kilometer long auto race takes place in Berland. The track is represented by a straight line as long as <span class="tex-span"><i>s</i></span> kilometers. There are <span class="tex-span"><i>n</i></span> cars taking part in the race, all of them start simultaneously at the very beginning of the track. For every car is known its behavior — the system of segments on each of which the speed of the car is constant. The <span class="tex-span"><i>j</i></span>-th segment of the <span class="tex-span"><i>i</i></span>-th car is pair <span class="tex-span">(<i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>, <i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>)</span>, where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is the car's speed on the whole segment in kilometers per hour and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is for how many hours the car had been driving at that speed. The segments are given in the order in which they are "being driven on" by the cars.</p><p>Your task is to find out how many times during the race some car managed to have a lead over another car. A lead is considered a situation when one car appears in front of another car. It is known, that all the leads happen instantly, i. e. there are no such time segment of positive length, during which some two cars drive "together". At one moment of time on one and the same point several leads may appear. In this case all of them should be taken individually. Meetings of cars at the start and finish are not considered to be counted as leads.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>s</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of cars and the length of the track in kilometers. Then follow <span class="tex-span"><i>n</i></span> lines — the description of the system of segments for each car. Every description starts with integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) — the number of segments in the system. Then <span class="tex-span"><i>k</i></span> space-separated pairs of integers are written. Each pair is the speed and time of the segment. These integers are positive and don't exceed 1000. It is guaranteed, that the sum of lengths of all segments (in kilometers) for each car equals to <span class="tex-span"><i>s</i></span>; and all the leads happen instantly.</p></div><div class="output-specification"><p>Print the single number — the number of times some car managed to take the lead over another car during the race.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100, 1 ≤ <i>s</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of cars and the length of the track in kilometers. Then follow <span class="tex-span"><i>n</i></span> lines — the description of the system of segments for each car. Every description starts with integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 100</span>) — the number of segments in the system. Then <span class="tex-span"><i>k</i></span> space-separated pairs of integers are written. Each pair is the speed and time of the segment. These integers are positive and don't exceed 1000. It is guaranteed, that the sum of lengths of all segments (in kilometers) for each car equals to <span class="tex-span"><i>s</i></span>; and all the leads happen instantly.</p>

## Output

<p>Print the single number — the number of times some car managed to take the lead over another car during the race.</p>





```input1
2 33
2 5 1 2 14
1 3 11

```




```input2
2 33
2 1 3 10 3
1 11 3

```




```input3
5 33
2 1 3 3 10
1 11 3
2 5 3 3 6
2 3 1 10 3
2 6 3 3 5

```




```output1
1

```




```output2
0

```




```output3
2

```


