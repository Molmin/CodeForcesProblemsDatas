## Description

<div><p>In a Berland's zoo there is an enclosure with camels. It is known that camels like to spit. Bob watched these interesting animals for the whole day and registered in his notepad where each animal spitted. Now he wants to know if in the zoo there are two camels, which spitted at each other. Help him to solve this task.</p><p>The trajectory of a camel's spit is an arc, i.e. if the camel in position <span class="tex-span"><i>x</i></span> spits <span class="tex-span"><i>d</i></span> meters right, he can hit only the camel in position <span class="tex-span"><i>x</i> + <i>d</i></span>, if such a camel exists.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the amount of camels in the zoo. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ |<i>d</i><sub class="lower-index"><i>i</i></sub>| ≤ 2·10<sup class="upper-index">4</sup></span>) — records in Bob's notepad. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a position of the <span class="tex-span"><i>i</i></span>-th camel, and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is a distance at which the <span class="tex-span"><i>i</i></span>-th camel spitted. Positive values of <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> correspond to the spits right, negative values correspond to the spits left. No two camels may stand in the same position.</p></div><div class="output-specification"><p>If there are two camels, which spitted at each other, output <span class="tex-font-style-tt">YES</span>. Otherwise, output <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the amount of camels in the zoo. Each of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ |<i>d</i><sub class="lower-index"><i>i</i></sub>| ≤ 2·10<sup class="upper-index">4</sup></span>) — records in Bob's notepad. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a position of the <span class="tex-span"><i>i</i></span>-th camel, and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is a distance at which the <span class="tex-span"><i>i</i></span>-th camel spitted. Positive values of <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> correspond to the spits right, negative values correspond to the spits left. No two camels may stand in the same position.</p>

## Output

<p>If there are two camels, which spitted at each other, output <span class="tex-font-style-tt">YES</span>. Otherwise, output <span class="tex-font-style-tt">NO</span>.</p>





```input1
2
0 1
1 -1

```




```input2
3
0 1
1 1
2 -2

```




```input3
5
2 -10
3 10
0 5
5 -5
10 1

```




```output1
YES

```




```output2
NO

```




```output3
YES

```


