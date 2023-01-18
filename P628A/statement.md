## Description

<div><p>A tennis tournament with <span class="tex-span"><i>n</i></span> participants is running. The participants are playing by an olympic system, so the winners move on and the losers drop out.</p><p>The tournament takes place in the following way (below, <span class="tex-span"><i>m</i></span> is the number of the participants of the current round):</p><ul> <li> let <span class="tex-span"><i>k</i></span> be the maximal power of the number <span class="tex-span">2</span> such that <span class="tex-span"><i>k</i> ≤ <i>m</i></span>, </li><li> <span class="tex-span"><i>k</i></span> participants compete in the current round and a half of them passes to the next round, the other <span class="tex-span"><i>m</i> - <i>k</i></span> participants pass to the next round directly, </li><li> when only one participant remains, the tournament finishes. </li></ul><p>Each match requires <span class="tex-span"><i>b</i></span> bottles of water for each participant and one bottle for the judge. Besides <span class="tex-span"><i>p</i></span> towels are given to each participant for the whole tournament.</p><p>Find the number of bottles and towels needed for the tournament.</p><p>Note that it's a tennis tournament so in each match two participants compete (one of them will win and the other will lose).</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>n</i>, <i>b</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>b</i>, <i>p</i> ≤ 500</span>) — the number of participants and the parameters described in the problem statement.</p></div><div class="output-specification"><p>Print two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the number of bottles and towels need for the tournament.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>n</i>, <i>b</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>b</i>, <i>p</i> ≤ 500</span>) — the number of participants and the parameters described in the problem statement.</p>

## Output

<p>Print two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> — the number of bottles and towels need for the tournament.</p>





```input1
5 2 3

```




```input2
8 2 4

```




```output1
20 15

```




```output2
35 32

```



## Note

<p>In the first example will be three rounds:</p><ol> <li> in the first round will be two matches and for each match <span class="tex-span">5</span> bottles of water are needed (two for each of the participants and one for the judge), </li><li> in the second round will be only one match, so we need another <span class="tex-span">5</span> bottles of water, </li><li> in the third round will also be only one match, so we need another <span class="tex-span">5</span> bottles of water. </li></ol><p>So in total we need <span class="tex-span">20</span> bottles of water.</p><p>In the second example no participant will move on to some round directly.</p>
