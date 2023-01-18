## Description

<div><p>Once archaeologists found <span class="tex-span"><i>m</i></span> mysterious papers, each of which had a pair of integers written on them. Ancient people were known to like writing down the indexes of the roads they walked along, as «<span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span>» or «<span class="tex-span"><i>b</i></span> <span class="tex-span"><i>a</i></span>», where <span class="tex-span"><i>a</i>, <i>b</i></span> are the indexes of two different cities joint by the road . It is also known that the mysterious papers are pages of two travel journals (those days a new journal was written for every new journey).</p><p>During one journey the traveler could walk along one and the same road several times in one or several directions but in that case he wrote a new entry for each time in his journal. Besides, the archaeologists think that the direction the traveler took on a road had no effect upon the entry: the entry that looks like «<span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span>» could refer to the road from <span class="tex-span"><i>a</i></span> to <span class="tex-span"><i>b</i></span> as well as to the road from <span class="tex-span"><i>b</i></span> to <span class="tex-span"><i>a</i></span>.</p><p>The archaeologists want to put the pages in the right order and reconstruct the two travel paths but unfortunately, they are bad at programming. That’s where you come in. Go help them!</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10000</span>). Each of the following <span class="tex-span"><i>m</i></span> lines describes one paper. Each description consists of two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10000</span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>).</p></div><div class="output-specification"><p>In the first line output the number <span class="tex-span"><i>L</i><sub class="lower-index">1</sub></span>. That is the length of the first path, i.e. the amount of papers in its description. In the following line output <span class="tex-span"><i>L</i><sub class="lower-index">1</sub></span> space-separated numbers — the indexes of the papers that describe the first path. In the third and fourth lines output similarly the length of the second path <span class="tex-span"><i>L</i><sub class="lower-index">2</sub></span> and the path itself. Both paths must contain at least one road, i.e. condition <span class="tex-span"><i>L</i><sub class="lower-index">1</sub> &gt; 0</span> and <span class="tex-span"><i>L</i><sub class="lower-index">2</sub> &gt; 0</span> must be met. The papers are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> according to the order of their appearance in the input file. The numbers should be output in the order in which the traveler passed the corresponding roads. If the answer is not unique, output any.</p><p>If it’s impossible to find such two paths, output «<span class="tex-font-style-tt">-1</span>».</p><p>Don’t forget that each paper should be used exactly once, i.e <span class="tex-span"><i>L</i><sub class="lower-index">1</sub> + <i>L</i><sub class="lower-index">2</sub> = <i>m</i></span>.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10000</span>). Each of the following <span class="tex-span"><i>m</i></span> lines describes one paper. Each description consists of two integers <span class="tex-span"><i>a</i>, <i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10000</span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>).</p>

## Output

<p>In the first line output the number <span class="tex-span"><i>L</i><sub class="lower-index">1</sub></span>. That is the length of the first path, i.e. the amount of papers in its description. In the following line output <span class="tex-span"><i>L</i><sub class="lower-index">1</sub></span> space-separated numbers — the indexes of the papers that describe the first path. In the third and fourth lines output similarly the length of the second path <span class="tex-span"><i>L</i><sub class="lower-index">2</sub></span> and the path itself. Both paths must contain at least one road, i.e. condition <span class="tex-span"><i>L</i><sub class="lower-index">1</sub> &gt; 0</span> and <span class="tex-span"><i>L</i><sub class="lower-index">2</sub> &gt; 0</span> must be met. The papers are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> according to the order of their appearance in the input file. The numbers should be output in the order in which the traveler passed the corresponding roads. If the answer is not unique, output any.</p><p>If it’s impossible to find such two paths, output «<span class="tex-font-style-tt">-1</span>».</p><p>Don’t forget that each paper should be used exactly once, i.e <span class="tex-span"><i>L</i><sub class="lower-index">1</sub> + <i>L</i><sub class="lower-index">2</sub> = <i>m</i></span>.</p>





```input1
2
4 5
4 3

```




```input2
1
1 2

```




```output1
1
2 
1
1

```




```output2
-1

```


