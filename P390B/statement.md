## Description

<div><p>Inna is a great piano player and Dima is a modest guitar player. Dima has recently written a song and they want to play it together. Of course, Sereja wants to listen to the song very much. </p><p>A song is a sequence of notes. Dima and Inna want to play each note at the same time. At that, they can play the <span class="tex-span"><i>i</i></span>-th note at volume <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>v</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span"><i>v</i></span> is an integer) both on the piano and the guitar. They should retain harmony, so the total volume with which the <span class="tex-span"><i>i</i></span>-th note was played on the guitar and the piano must equal <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. If Dima and Inna cannot play a note by the described rules, they skip it and Sereja's joy drops by 1. But if Inna and Dima play the <span class="tex-span"><i>i</i></span>-th note at volumes <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> correspondingly, Sereja's joy rises by <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>·<i>y</i><sub class="lower-index"><i>i</i></sub></span>. </p><p>Sereja has just returned home from the university and his current joy is 0. Help Dima and Inna play the song so as to maximize Sereja's total joy after listening to the whole song!</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of notes in the song. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p></div><div class="output-specification"><p>In a single line print an integer — the maximum possible joy Sereja feels after he listens to a song.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of notes in the song. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>.</p>

## Output

<p>In a single line print an integer — the maximum possible joy Sereja feels after he listens to a song.</p>





```input1
3
1 1 2
2 2 3

```




```input2
1
2
5

```




```output1
4

```




```output2
-1

```



## Note

<p>In the first sample, Dima and Inna play the first two notes at volume <span class="tex-span">1</span> (<span class="tex-span">1 + 1 = 2</span>, the condition holds), they should play the last note at volumes <span class="tex-span">1</span> and <span class="tex-span">2</span>. Sereja's total joy equals: <span class="tex-span">1·1 + 1·1 + 1·2 = 4</span>.</p><p>In the second sample, there is no such pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, that <span class="tex-span">1 ≤ <i>x</i>, <i>y</i> ≤ 2</span>, <span class="tex-span"><i>x</i> + <i>y</i> = 5</span>, so Dima and Inna skip a note. Sereja's total joy equals -1.</p>
