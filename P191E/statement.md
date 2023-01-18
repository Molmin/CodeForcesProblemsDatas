## Description

<div><p>It is dark times in Berland. Berlyand opposition, funded from a neighboring state, has organized a demonstration in Berland capital Bertown. Through the work of intelligence we know that the demonstrations are planned to last for <span class="tex-span"><i>k</i></span> days.</p><p>Fortunately, Berland has a special police unit, which can save the country. It has exactly <span class="tex-span"><i>n</i></span> soldiers numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Berland general, the commander of the detachment, must schedule the detachment's work in these difficult <span class="tex-span"><i>k</i></span> days. In each of these days, the general must send a certain number of police officers to disperse riots. Since the detachment is large and the general is not very smart, he can only select a set of all soldiers numbered from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, inclusive, where <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> are selected arbitrarily.</p><p>Now the general has exactly two problems. First, he cannot send the same group twice — then soldiers get bored and they rebel. Second, not all soldiers are equally reliable. Every soldier has a reliability of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The reliability of the detachment is counted as the sum of reliabilities of soldiers in it. The reliability of a single soldier can be negative, then when you include him in the detachment, he will only spoil things. The general is distinguished by his great greed and shortsightedness, so each day he sends to the dissolution the most reliable group of soldiers possible (that is, of all the groups that have not been sent yet).</p><p>The Berland Government has decided to know what would be the minimum reliability of the detachment, sent to disperse the demonstrations during these <span class="tex-span"><i>k</i></span> days. The general himself can not cope with such a difficult task. Help him to not embarrass himself in front of his superiors!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <img align="middle" class="tex-formula" src="file://4B8onoOT.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of soldiers in the detachment and the number of times somebody goes on duty.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, their absolute value doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> — the soldiers' reliabilities.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++, it is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams of the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print a single number — the sought minimum reliability of the groups that go on duty during these <span class="tex-span"><i>k</i></span> days.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <img align="middle" class="tex-formula" src="file://4B8onoOT.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of soldiers in the detachment and the number of times somebody goes on duty.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, their absolute value doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> — the soldiers' reliabilities.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++, it is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams of the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print a single number — the sought minimum reliability of the groups that go on duty during these <span class="tex-span"><i>k</i></span> days.</p>





```input1
3 4
1 4 2

```




```input2
4 6
2 -1 2 -1

```




```input3
8 10
1 -2 3 -4 5 -6 7 -8

```




```output1
4

```




```output2
1

```




```output3
2

```


