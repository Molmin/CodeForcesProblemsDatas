## Description

<div><p>Recently Vasya got interested in finding extra-terrestrial intelligence. He made a simple extra-terrestrial signals’ receiver and was keeping a record of the signals for <span class="tex-span"><i>n</i></span> days in a row. Each of those <span class="tex-span"><i>n</i></span> days Vasya wrote a 1 in his notebook if he had received a signal that day and a 0 if he hadn’t. Vasya thinks that he has found extra-terrestrial intelligence if there is a system in the way the signals has been received, i.e. if all the intervals between successive signals are equal. Otherwise, Vasya thinks that the signals were sent by some stupid aliens no one cares about. Help Vasya to deduce from the information given by the receiver if he has found extra-terrestrial intelligence or not.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — amount of days during which Vasya checked if there were any signals. The second line contains <span class="tex-span"><i>n</i></span> characters 1 or 0 — the record Vasya kept each of those <span class="tex-span"><i>n</i></span> days. It’s guaranteed that the given record sequence contains at least three 1s.</p></div><div class="output-specification"><p>If Vasya has found extra-terrestrial intelligence, output <span class="tex-font-style-tt">YES</span>, otherwise output <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — amount of days during which Vasya checked if there were any signals. The second line contains <span class="tex-span"><i>n</i></span> characters 1 or 0 — the record Vasya kept each of those <span class="tex-span"><i>n</i></span> days. It’s guaranteed that the given record sequence contains at least three 1s.</p>

## Output

<p>If Vasya has found extra-terrestrial intelligence, output <span class="tex-font-style-tt">YES</span>, otherwise output <span class="tex-font-style-tt">NO</span>.</p>





```input1
8
00111000

```




```input2
7
1001011

```




```input3
7
1010100

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


