## Description

<div><p>Serega loves fun. However, everyone has fun in the unique manner. Serega has fun by solving query problems. One day Fedor came up with such a problem.</p><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> positive integers and queries to it. The queries can be of two types:</p><ol> <li> Make a unit cyclic shift to the right on the segment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (both borders inclusive). That is rearrange elements of the array in the following manner:<center class="tex-equation"><span class="tex-span"><i>a</i>[<i>l</i>], <i>a</i>[<i>l</i> + 1], ..., <i>a</i>[<i>r</i> - 1], <i>a</i>[<i>r</i>] → <i>a</i>[<i>r</i>], <i>a</i>[<i>l</i>], <i>a</i>[<i>l</i> + 1], ..., <i>a</i>[<i>r</i> - 1].</span></center></li><li> Count how many numbers equal to <span class="tex-span"><i>k</i></span> are on the segment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> (both borders inclusive). </li></ol><p>Fedor hurried to see Serega enjoy the problem and Serega solved it really quickly. Let's see, can you solve it?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements of the array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ <i>n</i></span>).</p><p>The third line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. The next <span class="tex-span"><i>q</i></span> lines contain the queries.</p><p>As you need to respond to the queries online, the queries will be <span class="tex-font-style-bf">encoded</span>. A query of the first type will be given in format: <span class="tex-span">1</span> <span class="tex-span"><i>l</i>'<sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i>'<sub class="lower-index"><i>i</i></sub></span>. A query of the second type will be given in format: <span class="tex-span">2</span> <span class="tex-span"><i>l</i>'<sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i>'<sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>k</i>'<sub class="lower-index"><i>i</i></sub></span>. All the number in input are integer. They satisfy the constraints: <span class="tex-span">1 ≤ <i>l</i>'<sub class="lower-index"><i>i</i></sub>, <i>r</i>'<sub class="lower-index"><i>i</i></sub>, <i>k</i>'<sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>.</p><p>To decode the queries from the data given in input, you need to perform the following transformations:</p><center class="tex-equation"><span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = ((<i>l</i>'<sub class="lower-index"><i>i</i></sub> + <i>lastans</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1;&nbsp;<i>r</i><sub class="lower-index"><i>i</i></sub> = ((<i>r</i>'<sub class="lower-index"><i>i</i></sub> + <i>lastans</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1;&nbsp;<i>k</i><sub class="lower-index"><i>i</i></sub> = ((<i>k</i>'<sub class="lower-index"><i>i</i></sub> + <i>lastans</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1.</span></center><p>Where <span class="tex-span"><i>lastans</i></span> is the last reply to the query of the 2-nd type (initially, <span class="tex-span"><i>lastans</i> = 0</span>). If after transformation <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is greater than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, you must swap these values.</p></div><div class="output-specification"><p>For each query of the 2-nd type print the answer on a single line.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements of the array. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">1 ≤ <i>a</i>[<i>i</i>] ≤ <i>n</i></span>).</p><p>The third line contains a single integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of queries. The next <span class="tex-span"><i>q</i></span> lines contain the queries.</p><p>As you need to respond to the queries online, the queries will be <span class="tex-font-style-bf">encoded</span>. A query of the first type will be given in format: <span class="tex-span">1</span> <span class="tex-span"><i>l</i>'<sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i>'<sub class="lower-index"><i>i</i></sub></span>. A query of the second type will be given in format: <span class="tex-span">2</span> <span class="tex-span"><i>l</i>'<sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i>'<sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>k</i>'<sub class="lower-index"><i>i</i></sub></span>. All the number in input are integer. They satisfy the constraints: <span class="tex-span">1 ≤ <i>l</i>'<sub class="lower-index"><i>i</i></sub>, <i>r</i>'<sub class="lower-index"><i>i</i></sub>, <i>k</i>'<sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>.</p><p>To decode the queries from the data given in input, you need to perform the following transformations:</p><center class="tex-equation"><span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = ((<i>l</i>'<sub class="lower-index"><i>i</i></sub> + <i>lastans</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1;&nbsp;<i>r</i><sub class="lower-index"><i>i</i></sub> = ((<i>r</i>'<sub class="lower-index"><i>i</i></sub> + <i>lastans</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1;&nbsp;<i>k</i><sub class="lower-index"><i>i</i></sub> = ((<i>k</i>'<sub class="lower-index"><i>i</i></sub> + <i>lastans</i> - 1)&nbsp;<i>mod</i>&nbsp;<i>n</i>) + 1.</span></center><p>Where <span class="tex-span"><i>lastans</i></span> is the last reply to the query of the 2-nd type (initially, <span class="tex-span"><i>lastans</i> = 0</span>). If after transformation <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is greater than <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, you must swap these values.</p>

## Output

<p>For each query of the 2-nd type print the answer on a single line.</p>





```input1
7
6 6 2 7 4 2 5
7
1 3 6
2 2 4 2
2 2 4 7
2 2 2 5
1 2 6
1 1 4
2 1 7 3

```




```input2
8
8 4 2 2 7 7 8 8
8
1 8 8
2 8 1 7
1 8 1
1 7 3
2 8 8 3
1 1 4
1 2 7
1 4 5

```




```output1
2
1
0
0

```




```output2
2
0

```


