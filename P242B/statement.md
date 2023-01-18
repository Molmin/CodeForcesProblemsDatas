## Description

<div><p>A coordinate line has <span class="tex-span"><i>n</i></span> segments, the <span class="tex-span"><i>i</i></span>-th segment starts at the position <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and ends at the position <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. We will denote such a segment as <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>.</p><p>You have suggested that one of the defined segments covers all others. In other words, there is such segment in the given set, which contains all other ones. Now you want to test your assumption. Find in the given set the segment which covers all other segments, and print its number. If such a segment doesn't exist, print -1.</p><p>Formally we will assume that segment <span class="tex-span">[<i>a</i>, <i>b</i>]</span> covers segment <span class="tex-span">[<i>c</i>, <i>d</i>]</span>, if they meet this condition <span class="tex-span"><i>a</i> ≤ <i>c</i> ≤ <i>d</i> ≤ <i>b</i></span>. </p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of segments. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the segments. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>It is guaranteed that no two segments coincide.</p></div><div class="output-specification"><p>Print a single integer — the number of the segment that covers all other segments in the set. If there's no solution, print -1.</p><p>The segments are numbered starting from <span class="tex-span">1</span> in the order in which they appear in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of segments. Next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the segments. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the borders of the <span class="tex-span"><i>i</i></span>-th segment.</p><p>It is guaranteed that no two segments coincide.</p>

## Output

<p>Print a single integer — the number of the segment that covers all other segments in the set. If there's no solution, print -1.</p><p>The segments are numbered starting from <span class="tex-span">1</span> in the order in which they appear in the input.</p>





```input1
3
1 1
2 2
3 3

```




```input2
6
1 5
2 3
1 10
7 10
7 7
10 10

```




```output1
-1

```




```output2
3

```


