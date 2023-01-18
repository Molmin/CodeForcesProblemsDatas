## Description

<div><p>Polycarpus is an amateur programmer. Now he is analyzing a friend's program. He has already found there the function <span class="tex-font-style-tt">rangeIncrement(l, r)</span>, that adds <span class="tex-font-style-tt">1</span> to each element of some array <span class="tex-span"><i>a</i></span> for all indexes in the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>. In other words, this function does the following: </p><pre class="verbatim"><br>function rangeIncrement(l, r)<br>    for i := l .. r do<br>        a[i] = a[i] + 1<br></pre><p>Polycarpus knows the state of the array <span class="tex-span"><i>a</i></span> after a series of function calls. He wants to determine the minimum number of function calls that lead to such state. In addition, he wants to find what function calls are needed in this case. It is guaranteed that the required number of calls does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>Before calls of function <span class="tex-font-style-tt">rangeIncrement(l, r)</span> all array elements equal zero.</p></div><div class="input-specification"><p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the array <span class="tex-span"><i>a</i>[1... <i>n</i>]</span>. </p><p>The second line contains its integer space-separated elements, <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">5</sup></span>) after some series of function calls <span class="tex-font-style-tt">rangeIncrement(l, r)</span>. </p><p>It is guaranteed that at least one element of the array is positive. It is guaranteed that the answer contains no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> calls of function <span class="tex-font-style-tt">rangeIncrement(l, r)</span>.</p></div><div class="output-specification"><p>Print on the first line <span class="tex-span"><i>t</i></span> — the minimum number of calls of function <span class="tex-font-style-tt">rangeIncrement(l, r)</span>, that lead to the array from the input data. It is guaranteed that this number will turn out not more than <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>Then print <span class="tex-span"><i>t</i></span> lines — the descriptions of function calls, one per line. Each line should contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the arguments of the <span class="tex-span"><i>i</i></span>-th call <span class="tex-font-style-tt">rangeIncrement(l, r)</span>. Calls can be applied in any order.</p><p>If there are multiple solutions, you are allowed to print any of them.</p></div>

## Input

<p>The first input line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the array <span class="tex-span"><i>a</i>[1... <i>n</i>]</span>. </p><p>The second line contains its integer space-separated elements, <span class="tex-span"><i>a</i>[1], <i>a</i>[2], ..., <i>a</i>[<i>n</i>]</span> (<span class="tex-span">0 ≤ <i>a</i>[<i>i</i>] ≤ 10<sup class="upper-index">5</sup></span>) after some series of function calls <span class="tex-font-style-tt">rangeIncrement(l, r)</span>. </p><p>It is guaranteed that at least one element of the array is positive. It is guaranteed that the answer contains no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> calls of function <span class="tex-font-style-tt">rangeIncrement(l, r)</span>.</p>

## Output

<p>Print on the first line <span class="tex-span"><i>t</i></span> — the minimum number of calls of function <span class="tex-font-style-tt">rangeIncrement(l, r)</span>, that lead to the array from the input data. It is guaranteed that this number will turn out not more than <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>Then print <span class="tex-span"><i>t</i></span> lines — the descriptions of function calls, one per line. Each line should contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the arguments of the <span class="tex-span"><i>i</i></span>-th call <span class="tex-font-style-tt">rangeIncrement(l, r)</span>. Calls can be applied in any order.</p><p>If there are multiple solutions, you are allowed to print any of them.</p>





```input1
6
1 2 1 1 4 1

```




```input2
5
1 0 1 0 1

```




```output1
5
2 2
5 5
5 5
5 5
1 6

```




```output2
3
1 1
3 3
5 5

```



## Note

<p>The first sample requires a call for the entire array, and four additional calls:</p><ul> <li> one for the segment [2,2] (i.e. the second element of the array), </li><li> three for the segment [5,5] (i.e. the fifth element of the array). </li></ul>
