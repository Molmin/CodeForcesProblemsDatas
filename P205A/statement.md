## Description

<div><p>The Little Elephant loves Ukraine very much. Most of all he loves town Rozdol (ukr. "Rozdil").</p><p>However, Rozdil is dangerous to settle, so the Little Elephant wants to go to some other town. The Little Elephant doesn't like to spend much time on travelling, so for his journey he will choose a town that needs minimum time to travel to. If there are multiple such cities, then the Little Elephant won't go anywhere.</p><p>For each town except for Rozdil you know the time needed to travel to this town. Find the town the Little Elephant will go to or print "<span class="tex-font-style-tt">Still Rozdil</span>", if he stays in Rozdil.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cities. The next line contains <span class="tex-span"><i>n</i></span> integers, separated by single spaces: the <span class="tex-span"><i>i</i></span>-th integer represents the time needed to go from town Rozdil to the <span class="tex-span"><i>i</i></span>-th town. The time values are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>You can consider the cities numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. Rozdil is not among the numbered cities.</p></div><div class="output-specification"><p>Print the answer on a single line — the number of the town the Little Elephant will go to. If there are multiple cities with minimum travel time, print "<span class="tex-font-style-tt">Still Rozdil</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cities. The next line contains <span class="tex-span"><i>n</i></span> integers, separated by single spaces: the <span class="tex-span"><i>i</i></span>-th integer represents the time needed to go from town Rozdil to the <span class="tex-span"><i>i</i></span>-th town. The time values are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>You can consider the cities numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. Rozdil is not among the numbered cities.</p>

## Output

<p>Print the answer on a single line — the number of the town the Little Elephant will go to. If there are multiple cities with minimum travel time, print "<span class="tex-font-style-tt">Still Rozdil</span>" (without the quotes).</p>





```input1
2
7 4

```




```input2
7
7 4 47 100 4 9 12

```




```output1
2

```




```output2
Still Rozdil

```



## Note

<p>In the first sample there are only two cities where the Little Elephant can go. The travel time for the first town equals <span class="tex-span">7</span>, to the second one — <span class="tex-span">4</span>. The town which is closest to Rodzil (the only one) is the second one, so the answer is <span class="tex-span">2</span>.</p><p>In the second sample the closest cities are cities two and five, the travelling time to both of them equals <span class="tex-span">4</span>, so the answer is "<span class="tex-font-style-tt">Still Rozdil</span>".</p>
