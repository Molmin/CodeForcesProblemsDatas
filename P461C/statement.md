## Description

<div><p>Appleman has a very big sheet of paper. This sheet has a form of rectangle with dimensions <span class="tex-span">1 × <i>n</i></span>. Your task is help Appleman with folding of such a sheet. Actually, you need to perform <span class="tex-span"><i>q</i></span> queries. Each query will have one of the following types:</p><ol> <li> Fold the sheet of paper at position <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. After this query the leftmost part of the paper with dimensions <span class="tex-span">1 × <i>p</i><sub class="lower-index"><i>i</i></sub></span> must be above the rightmost part of the paper with dimensions <span class="tex-span">1 × ([<i>current</i>&nbsp;<i>width</i>&nbsp;<i>of</i>&nbsp;<i>sheet</i>] - <i>p</i><sub class="lower-index"><i>i</i></sub>)</span>. </li><li> Count what is the total width of the paper pieces, if we will make two described later cuts and consider only the pieces between the cuts. We will make one cut at distance <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> from the left border of the current sheet of paper and the other at distance <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> from the left border of the current sheet of paper. </li></ol><p>Please look at the explanation of the first test example for better understanding of the problem.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1  ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the width of the paper and the number of queries.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains one of the described queries in the following format:</p><ul> <li> "<span class="tex-span">1</span> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>" <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; [<i>current</i>&nbsp;<i>width</i>&nbsp;<i>of</i>&nbsp;<i>sheet</i>])</span> — the first type query. </li><li> "<span class="tex-span">2</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>" <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ [<i>current</i>&nbsp;<i>width</i>&nbsp;<i>of</i>&nbsp;<i>sheet</i>])</span> — the second type query. </li></ul></div><div class="output-specification"><p>For each query of the second type, output the answer.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1  ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the width of the paper and the number of queries.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines contains one of the described queries in the following format:</p><ul> <li> "<span class="tex-span">1</span> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>" <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; [<i>current</i>&nbsp;<i>width</i>&nbsp;<i>of</i>&nbsp;<i>sheet</i>])</span> — the first type query. </li><li> "<span class="tex-span">2</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>" <span class="tex-span">(0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ [<i>current</i>&nbsp;<i>width</i>&nbsp;<i>of</i>&nbsp;<i>sheet</i>])</span> — the second type query. </li></ul>

## Output

<p>For each query of the second type, output the answer.</p>





```input1
7 4
1 3
1 2
2 0 1
2 1 2

```




```input2
10 9
2 2 9
1 1
2 0 1
1 8
2 0 8
1 2
2 1 3
1 4
2 2 4

```




```output1
4
3

```




```output2
7
2
10
4
5

```



## Note

<p>The pictures below show the shapes of the paper during the queries of the first example:</p><center> <img class="tex-graphics" src="file://fPxklZfE.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After the first fold operation the sheet has width equal to <span class="tex-span">4</span>, after the second one the width of the sheet equals to <span class="tex-span">2</span>.</p>
