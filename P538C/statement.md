## Description

<div><p>A tourist hiked along the mountain range. The hike lasted for <span class="tex-span"><i>n</i></span> days, during each day the tourist noted height above the sea level. On the <span class="tex-span"><i>i</i></span>-th day height was equal to some integer <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. The tourist pick smooth enough route for his hike, meaning that the between any two consecutive days height changes by at most 1, i.e. for all <span class="tex-span"><i>i</i></span>'s from 1 to <span class="tex-span"><i>n</i> - 1</span> the inequality <span class="tex-span">|<i>h</i><sub class="lower-index"><i>i</i></sub> - <i>h</i><sub class="lower-index"><i>i</i> + 1</sub>| ≤ 1</span> holds.</p><p>At the end of the route the tourist rafted down a mountain river and some notes in the journal were washed away. Moreover, the numbers in the notes could have been distorted. Now the tourist wonders what could be the maximum height during his hike. Help him restore the maximum possible value of the maximum height throughout the hike or determine that the notes were so much distorted that they do not represent any possible height values that meet limits <span class="tex-span">|<i>h</i><sub class="lower-index"><i>i</i></sub> - <i>h</i><sub class="lower-index"><i>i</i> + 1</sub>| ≤ 1</span>.</p></div><div class="input-specification"><p>The first line contains two space-separated numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days of the hike and the number of notes left in the journal.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>d</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>d</i><sub class="lower-index"><i>i</i></sub></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the number of the day when the <span class="tex-span"><i>i</i></span>-th note was made and height on the <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>-th day. It is guaranteed that the notes are given in the chronological order, i.e. for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>m</i> - 1</span> the following condition holds: <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>d</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p></div><div class="output-specification"><p>If the notes aren't contradictory, print a single integer — the maximum possible height value throughout the whole route.</p><p>If the notes do not correspond to any set of heights, print a single word '<span class="tex-font-style-tt">IMPOSSIBLE</span>' (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated numbers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">8</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of days of the hike and the number of notes left in the journal.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two space-separated integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index"><i>d</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>d</i><sub class="lower-index"><i>i</i></sub></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the number of the day when the <span class="tex-span"><i>i</i></span>-th note was made and height on the <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>-th day. It is guaranteed that the notes are given in the chronological order, i.e. for all <span class="tex-span"><i>i</i></span> from 1 to <span class="tex-span"><i>m</i> - 1</span> the following condition holds: <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>d</i><sub class="lower-index"><i>i</i> + 1</sub></span>.</p>

## Output

<p>If the notes aren't contradictory, print a single integer — the maximum possible height value throughout the whole route.</p><p>If the notes do not correspond to any set of heights, print a single word '<span class="tex-font-style-tt">IMPOSSIBLE</span>' (without the quotes).</p>





```input1
8 2
2 0
7 0

```




```input2
8 3
2 0
7 0
8 3

```




```output1
2

```




```output2
IMPOSSIBLE

```



## Note

<p>For the first sample, an example of a correct height sequence with a maximum of 2: <span class="tex-span">(0, 0, 1, 2, 1, 1, 0, 1)</span>.</p><p>In the second sample the inequality between <span class="tex-span"><i>h</i><sub class="lower-index">7</sub></span> and <span class="tex-span"><i>h</i><sub class="lower-index">8</sub></span> does not hold, thus the information is inconsistent.</p>
