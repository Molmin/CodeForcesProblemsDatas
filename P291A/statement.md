## Description

<div><p>Polycarpus is the director of a large corporation. There are <span class="tex-span"><i>n</i></span> secretaries working for the corporation, each of them corresponds via the famous Spyke VoIP system during the day. We know that when two people call each other via Spyke, the Spyke network assigns a unique ID to this call, a positive integer session number.</p><p>One day Polycarpus wondered which secretaries are talking via the Spyke and which are not. For each secretary, he wrote out either the session number of his call or a 0 if this secretary wasn't talking via Spyke at that moment.</p><p>Help Polycarpus analyze these data and find out the number of pairs of secretaries that are talking. If Polycarpus has made a mistake in the data and the described situation could not have taken place, say so.</p><p>Note that the secretaries can correspond via Spyke not only with each other, but also with the people from other places. Also, Spyke conferences aren't permitted — that is, one call connects exactly two people.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the number of secretaries in Polycarpus's corporation. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Number <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> equals the number of the call session of the <span class="tex-span"><i>i</i></span>-th secretary, if the secretary is talking via Spyke, or zero otherwise.</p><p>Consider the secretaries indexed from 1 to <span class="tex-span"><i>n</i></span> in some way.</p></div><div class="output-specification"><p>Print a single integer — the number of pairs of chatting secretaries, or <span class="tex-font-style-tt">-1</span> if Polycarpus's got a mistake in his records and the described situation could not have taken place.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup>)</span> — the number of secretaries in Polycarpus's corporation. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. Number <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> equals the number of the call session of the <span class="tex-span"><i>i</i></span>-th secretary, if the secretary is talking via Spyke, or zero otherwise.</p><p>Consider the secretaries indexed from 1 to <span class="tex-span"><i>n</i></span> in some way.</p>

## Output

<p>Print a single integer — the number of pairs of chatting secretaries, or <span class="tex-font-style-tt">-1</span> if Polycarpus's got a mistake in his records and the described situation could not have taken place.</p>





```input1
6
0 1 7 1 7 10

```




```input2
3
1 1 1

```




```input3
1
0

```




```output1
2

```




```output2
-1

```




```output3
0

```



## Note

<p>In the first test sample there are two Spyke calls between secretaries: secretary 2 and secretary 4, secretary 3 and secretary 5.</p><p>In the second test sample the described situation is impossible as conferences aren't allowed.</p>
