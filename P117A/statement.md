## Description

<div><p>And now the numerous qualifying tournaments for one of the most prestigious Russian contests <span class="tex-font-style-it">Russian Codec Cup</span> are over. All <span class="tex-span"><i>n</i></span> participants who have made it to the finals found themselves in a huge <span class="tex-span"><i>m</i></span>-floored <span class="tex-span">10<sup class="upper-index">8</sup></span>-star hotel. Of course the first thought to come in a place like this is "How about checking out the elevator?".</p><p>The hotel's elevator moves between floors according to one never changing scheme. Initially (at the moment of time <span class="tex-span">0</span>) the elevator is located on the <span class="tex-span">1</span>-st floor, then it moves to the <span class="tex-span">2</span>-nd floor, then — to the <span class="tex-span">3</span>-rd floor and so on until it reaches the <span class="tex-span"><i>m</i></span>-th floor. After that the elevator moves to floor <span class="tex-span"><i>m</i> - 1</span>, then to floor <span class="tex-span"><i>m</i> - 2</span>, and so on until it reaches the first floor. This process is repeated infinitely. We know that the elevator has infinite capacity; we also know that on every floor people get on the elevator immediately. Moving between the floors takes a unit of time.</p><p>For each of the <span class="tex-span"><i>n</i></span> participant you are given <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, which represents the floor where the <span class="tex-span"><i>i</i></span>-th participant starts, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, which represents the floor the <span class="tex-span"><i>i</i></span>-th participant wants to reach, and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, which represents the time when the <span class="tex-span"><i>i</i></span>-th participant starts on the floor <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>For each participant print the minimum time of his/her arrival to the floor <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>If the elevator stops on the floor <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> at the time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, then the <span class="tex-span"><i>i</i></span>-th participant can enter the elevator immediately. If the participant starts on the floor <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and that's the floor he wanted to reach initially (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>f</i><sub class="lower-index"><i>i</i></sub></span>), then the time of arrival to the floor <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> for this participant is considered equal to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10<sup class="upper-index">8</sup></span>). </p><p>Next <span class="tex-span"><i>n</i></span> lines contain information about the participants in the form of three space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), described in the problem statement.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines each containing one integer — the time of the arrival for each participant to the required floor.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10<sup class="upper-index">8</sup></span>). </p><p>Next <span class="tex-span"><i>n</i></span> lines contain information about the participants in the form of three space-separated integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub>, <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i>, 0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>), described in the problem statement.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines each containing one integer — the time of the arrival for each participant to the required floor.</p>





```input1
7 4
2 4 3
1 2 0
2 2 0
1 2 1
4 3 5
1 2 2
4 2 0

```




```input2
5 5
1 5 4
1 3 1
1 3 4
3 1 5
4 2 5

```




```output1
9
1
0
7
10
7
5

```




```output2
12
10
10
8
7

```



## Note

<p>Let's consider the first sample. The first participant starts at floor <span class="tex-span"><i>s</i> = 2</span> by the time equal to <span class="tex-span"><i>t</i> = 3</span>. To get to the floor <span class="tex-span"><i>f</i> = 4</span>, he has to wait until the time equals <span class="tex-span">7</span>, that's the time when the elevator will go upwards for the second time. Then the first participant should get on the elevator and go two floors up. In this case the first participant gets to the floor <span class="tex-span"><i>f</i></span> at time equal to <span class="tex-span">9</span>. The second participant starts at the time <span class="tex-span"><i>t</i> = 0</span> on the floor <span class="tex-span"><i>s</i> = 1</span>, enters the elevator immediately, and arrives to the floor <span class="tex-span"><i>f</i> = 2</span>. The third participant doesn't wait for the elevator, because he needs to arrive to the same floor where he starts.</p>
