## Description

<div><p>The elections to Berland parliament are happening today. Voting is in full swing!</p><p>Totally there are <span class="tex-span"><i>n</i></span> candidates, they are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Based on election results <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) top candidates will take seats in the parliament.</p><p>After the end of the voting the number of votes for each candidate is calculated. In the resulting table the candidates are ordered by the number of votes. In case of tie (equal number of votes) they are ordered by the time of the last vote given. The candidate with ealier last vote stands higher in the resulting table.</p><p>So in the resulting table candidates are sorted by the number of votes (more votes stand for the higher place) and if two candidates have equal number of votes they are sorted by the time of last vote (earlier last vote stands for the higher place).</p><p>There is no way for a candidate with zero votes to take a seat in the parliament. So it is possible that less than <span class="tex-span"><i>k</i></span> candidates will take a seat in the parliament.</p><p>In Berland there are <span class="tex-span"><i>m</i></span> citizens who can vote. Each of them will vote for some candidate. Each citizen will give a vote to exactly one of <span class="tex-span"><i>n</i></span> candidates. There is no option "against everyone" on the elections. It is not accepted to spoil bulletins or not to go to elections. So each of <span class="tex-span"><i>m</i></span> citizens will vote for exactly one of <span class="tex-span"><i>n</i></span> candidates.</p><p>At the moment <span class="tex-span"><i>a</i></span> citizens have voted already (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>m</i></span>). This is an open election, so for each citizen it is known the candidate for which the citizen has voted. Formally, the <span class="tex-span"><i>j</i></span>-th citizen voted for the candidate <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub></span>. The citizens who already voted are numbered in chronological order; i.e. the <span class="tex-span">(<i>j</i> + 1)</span>-th citizen voted after the <span class="tex-span"><i>j</i></span>-th.</p><p>The remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens will vote before the end of elections, each of them will vote for one of <span class="tex-span"><i>n</i></span> candidates.</p><p>Your task is to determine for each of <span class="tex-span"><i>n</i></span> candidates one of the three possible outcomes:</p><ul> <li> a candidate will be elected to the parliament regardless of votes of the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens; </li><li> a candidate has chance to be elected to the parliament after all <span class="tex-span"><i>n</i></span> citizens have voted; </li><li> a candidate has no chances to be elected to the parliament regardless of votes of the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens. </li></ul></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>a</i> ≤ <i>m</i></span>) — the number of candidates, the number of seats in the parliament, the number of Berland citizens and the number of citizens who already have voted.</p><p>The second line contains a sequence of <span class="tex-span"><i>a</i></span> integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>a</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub></span> is the candidate for which the <span class="tex-span"><i>j</i></span>-th citizen has voted. Citizens who already voted are numbered in increasing order of voting times.</p></div><div class="output-specification"><p>Print the sequence consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> where:</p><ul> <li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 1</span> means that the <span class="tex-span"><i>i</i></span>-th candidate is guaranteed to take seat in the parliament regardless of votes of the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 2</span> means that the <span class="tex-span"><i>i</i></span>-th candidate has a chance to take a seat in the parliament, i.e. the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens can vote in such a way that the candidate will take a seat in the parliament; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 3</span> means that the <span class="tex-span"><i>i</i></span>-th candidate will not take a seat in the parliament regardless of votes of the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens. </li></ul></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>a</i> ≤ <i>m</i></span>) — the number of candidates, the number of seats in the parliament, the number of Berland citizens and the number of citizens who already have voted.</p><p>The second line contains a sequence of <span class="tex-span"><i>a</i></span> integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>a</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>g</i><sub class="lower-index"><i>j</i></sub></span> is the candidate for which the <span class="tex-span"><i>j</i></span>-th citizen has voted. Citizens who already voted are numbered in increasing order of voting times.</p>

## Output

<p>Print the sequence consisting of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, ..., <i>r</i><sub class="lower-index"><i>n</i></sub></span> where:</p><ul> <li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 1</span> means that the <span class="tex-span"><i>i</i></span>-th candidate is guaranteed to take seat in the parliament regardless of votes of the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 2</span> means that the <span class="tex-span"><i>i</i></span>-th candidate has a chance to take a seat in the parliament, i.e. the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens can vote in such a way that the candidate will take a seat in the parliament; </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> = 3</span> means that the <span class="tex-span"><i>i</i></span>-th candidate will not take a seat in the parliament regardless of votes of the remaining <span class="tex-span"><i>m</i> - <i>a</i></span> citizens. </li></ul>





```input1
3 1 5 4
1 2 1 3

```




```input2
3 1 5 3
1 3 1

```




```input3
3 2 5 3
1 3 1

```




```output1
1 3 3
```




```output2
2 3 2
```




```output3
1 2 2
```


