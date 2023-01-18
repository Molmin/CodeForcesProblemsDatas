## Description

<div><p>Two semifinals have just been in the running tournament. Each semifinal had <span class="tex-span"><i>n</i></span> participants. There are <span class="tex-span"><i>n</i></span> participants advancing to the finals, they are chosen as follows: from each semifinal, we choose <span class="tex-span"><i>k</i></span> people (<span class="tex-span">0 ≤ 2<i>k</i> ≤ <i>n</i></span>) who showed the best result in their semifinals and all other places in the finals go to the people who haven't ranked in the top <span class="tex-span"><i>k</i></span> in their semifinal but got to the <span class="tex-span"><i>n</i> - 2<i>k</i></span> of the best among the others.</p><p>The tournament organizers hasn't yet determined the <span class="tex-span"><i>k</i></span> value, so the participants want to know who else has any chance to get to the finals and who can go home.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of participants in each semifinal.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the results of the <span class="tex-span"><i>i</i></span>-th participant (the number of milliseconds he needs to cover the semifinals distance) of the first and second semifinals, correspondingly. All results are distinct. Sequences <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> are sorted in ascending order, i.e. in the order the participants finished in the corresponding semifinal.</p></div><div class="output-specification"><p>Print two strings consisting of <span class="tex-span"><i>n</i></span> characters, each equals either "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>". The first line should correspond to the participants of the first semifinal, the second line should correspond to the participants of the second semifinal. The <span class="tex-span"><i>i</i></span>-th character in the <span class="tex-span"><i>j</i></span>-th line should equal "<span class="tex-font-style-tt">1</span>" if the <span class="tex-span"><i>i</i></span>-th participant of the <span class="tex-span"><i>j</i></span>-th semifinal has any chances to advance to the finals, otherwise it should equal a "<span class="tex-font-style-tt">0</span>".</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of participants in each semifinal.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the results of the <span class="tex-span"><i>i</i></span>-th participant (the number of milliseconds he needs to cover the semifinals distance) of the first and second semifinals, correspondingly. All results are distinct. Sequences <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> are sorted in ascending order, i.e. in the order the participants finished in the corresponding semifinal.</p>

## Output

<p>Print two strings consisting of <span class="tex-span"><i>n</i></span> characters, each equals either "<span class="tex-font-style-tt">0</span>" or "<span class="tex-font-style-tt">1</span>". The first line should correspond to the participants of the first semifinal, the second line should correspond to the participants of the second semifinal. The <span class="tex-span"><i>i</i></span>-th character in the <span class="tex-span"><i>j</i></span>-th line should equal "<span class="tex-font-style-tt">1</span>" if the <span class="tex-span"><i>i</i></span>-th participant of the <span class="tex-span"><i>j</i></span>-th semifinal has any chances to advance to the finals, otherwise it should equal a "<span class="tex-font-style-tt">0</span>".</p>





```input1
4
9840 9920
9860 9980
9930 10020
10040 10090

```




```input2
4
9900 9850
9940 9930
10000 10020
10060 10110

```




```output1
1110
1100

```




```output2
1100
1100

```



## Note

<p>Consider the first sample. Each semifinal has 4 participants. The results of the first semifinal are 9840, 9860, 9930, 10040. The results of the second semifinal are 9920, 9980, 10020, 10090.</p><ul> <li> If <span class="tex-span"><i>k</i> = 0</span>, the finalists are determined by the time only, so players 9840, 9860, 9920 and 9930 advance to the finals. </li><li> If <span class="tex-span"><i>k</i> = 1</span>, the winners from both semifinals move to the finals (with results 9840 and 9920), and the other places are determined by the time (these places go to the sportsmen who run the distance in 9860 and 9930 milliseconds). </li><li> If <span class="tex-span"><i>k</i> = 2</span>, then first and second places advance from each seminfial, these are participants with results 9840, 9860, 9920 and 9980 milliseconds. </li></ul>
