## Description

<div><p>You've gotten an <span class="tex-span"><i>n</i> × <i>m</i></span> sheet of squared paper. Some of its squares are painted. Let's mark the set of all painted squares as <span class="tex-span"><i>A</i></span>. Set <span class="tex-span"><i>A</i></span> is connected. Your task is to find the minimum number of squares that we can delete from set <span class="tex-span"><i>A</i></span> to make it not connected.</p><p>A set of painted squares is called <span class="tex-font-style-it">connected</span>, if for every two squares <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> from this set there is a sequence of squares from the set, beginning in <span class="tex-span"><i>a</i></span> and ending in <span class="tex-span"><i>b</i></span>, such that in this sequence any square, except for the last one, shares a common side with the square that follows next in the sequence. An empty set and a set consisting of exactly one square are connected by definition.</p></div><div class="input-specification"><p>The first input line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the sizes of the sheet of paper. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the sheet of paper: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals either "#", if the corresponding square is painted (belongs to set <span class="tex-span"><i>A</i></span>), or equals "." if the corresponding square is not painted (does not belong to set <span class="tex-span"><i>A</i></span>). It is guaranteed that the set of all painted squares <span class="tex-span"><i>A</i></span> is connected and isn't empty.</p></div><div class="output-specification"><p>On the first line print the minimum number of squares that need to be deleted to make set <span class="tex-span"><i>A</i></span> not connected. If it is impossible, print -1. </p></div>

## Input

<p>The first input line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 50</span>) — the sizes of the sheet of paper. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>m</i></span> characters — the description of the sheet of paper: the <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line equals either "#", if the corresponding square is painted (belongs to set <span class="tex-span"><i>A</i></span>), or equals "." if the corresponding square is not painted (does not belong to set <span class="tex-span"><i>A</i></span>). It is guaranteed that the set of all painted squares <span class="tex-span"><i>A</i></span> is connected and isn't empty.</p>

## Output

<p>On the first line print the minimum number of squares that need to be deleted to make set <span class="tex-span"><i>A</i></span> not connected. If it is impossible, print -1. </p>





```input1
5 4
####
#..#
#..#
#..#
####

```




```input2
5 5
#####
#...#
#####
#...#
#####

```




```output1
2

```




```output2
2

```



## Note

<p>In the first sample you can delete any two squares that do not share a side. After that the set of painted squares is not connected anymore.</p><p>The note to the second sample is shown on the figure below. To the left there is a picture of the initial set of squares. To the right there is a set with deleted squares. The deleted squares are marked with crosses. </p><center> <img class="tex-graphics" src="file://zzOFqNSf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
