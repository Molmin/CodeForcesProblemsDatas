## Description

<div><p>Andrew skipped lessons on the subject 'Algorithms and Data Structures' for the entire term. When he came to the final test, the teacher decided to give him a difficult task as a punishment.</p><p>The teacher gave Andrew an array of <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. After that he asked Andrew for each <span class="tex-span"><i>k</i></span> from 1 to <span class="tex-span"><i>n</i> - 1</span> to build a <span class="tex-span"><i>k</i></span>-ary heap on the array and count the number of elements for which the property of the minimum-rooted heap is violated, i.e. the value of an element is less than the value of its parent.</p><p>Andrew looked up on the Wikipedia that a <span class="tex-span"><i>k</i></span>-ary heap is a rooted tree with vertices in elements of the array. If the elements of the array are indexed from 1 to <span class="tex-span"><i>n</i></span>, then the children of element <span class="tex-span"><i>v</i></span> are elements with indices <span class="tex-span"><i>k</i>(<i>v</i> - 1) + 2</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>kv</i> + 1</span> (if some of these elements lie outside the borders of the array, the corresponding children are absent). In any <span class="tex-span"><i>k</i></span>-ary heap every element except for the first one has exactly one parent; for the element 1 the parent is absent (this element is the <span class="tex-font-style-it">root</span> of the heap). Denote <span class="tex-span"><i>p</i>(<i>v</i>)</span> as the number of the parent of the element with the number <span class="tex-span"><i>v</i></span>. Let's say that for a non-root element <span class="tex-span"><i>v</i></span> the <span class="tex-font-style-it">property of the heap is violated</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>v</i></sub> &lt; <i>a</i><sub class="lower-index"><i>p</i>(<i>v</i>)</sub></span>.</p><p>Help Andrew cope with the task!</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>in a single line print <span class="tex-span"><i>n</i> - 1</span> integers, separate the consecutive numbers with a single space — the number of elements for which the property of the <span class="tex-span"><i>k</i></span>-ary heap is violated, for <span class="tex-span"><i>k</i> = 1</span>, <span class="tex-span">2</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>n</i> - 1</span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>in a single line print <span class="tex-span"><i>n</i> - 1</span> integers, separate the consecutive numbers with a single space — the number of elements for which the property of the <span class="tex-span"><i>k</i></span>-ary heap is violated, for <span class="tex-span"><i>k</i> = 1</span>, <span class="tex-span">2</span>, <span class="tex-span">...</span>, <span class="tex-span"><i>n</i> - 1</span>.</p>





```input1
5
1 5 4 3 2

```




```input2
6
2 2 2 2 2 2

```




```output1
3 2 1 0

```




```output2
0 0 0 0 0

```



## Note

<p>Pictures with the heaps for the first sample are given below; elements for which the property of the heap is violated are marked with red.</p><center> <img class="tex-graphics" src="file://c7RPGaZz.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://kFKisNCF.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://2tVOOeIQ.png" style="max-width: 100.0%;max-height: 100.0%;"> <img class="tex-graphics" src="file://q2SNozRP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample all elements are equal, so the property holds for all pairs.</p>
