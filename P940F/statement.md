## Description

<div><p><span class="tex-font-style-it">You come home and fell some unpleasant smell. Where is it coming from?</span></p><p>You are given an array <span class="tex-span"><i>a</i></span>. You have to answer the following queries: </p><ol> <li> You are given two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>. Let <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> be the number of occurrences of <span class="tex-span"><i>i</i></span> in <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i>: <i>r</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i>: <i>r</i></sub></span> is the subarray of <span class="tex-span"><i>a</i></span> from <span class="tex-span"><i>l</i></span>-th element to <span class="tex-span"><i>r</i></span>-th inclusive. Find the <span class="tex-font-style-bf">Mex</span> of <span class="tex-span">{<i>c</i><sub class="lower-index">0</sub>, <i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index">10<sup class="upper-index">9</sup></sub>}</span> </li><li> You are given two integers <span class="tex-span"><i>p</i></span> to <span class="tex-span"><i>x</i></span>. Change <span class="tex-span"><i>a</i><sub class="lower-index"><i>p</i></sub></span> to <span class="tex-span"><i>x</i></span>. </li></ol><p>The <span class="tex-font-style-bf">Mex</span> of a multiset of numbers is the smallest non-negative integer <span class="tex-font-style-bf">not in</span> the set.</p><p>Note that in this problem all elements of <span class="tex-span"><i>a</i></span> are positive, which means that <span class="tex-span"><i>c</i><sub class="lower-index">0</sub></span> = 0 and <span class="tex-span">0</span> is never the answer for the query of the second type.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 100 000</span>)&nbsp;— the length of the array and the number of queries respectively.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers&nbsp;— <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines describes a single query.</p><p>The first type of query is described by three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>&nbsp;— the bounds of the subarray.</p><p>The second type of query is described by three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> is the index of the element, which must be changed and <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> is the new value.</p></div><div class="output-specification"><p>For each query of the first type output a single integer &nbsp;— the <span class="tex-font-style-bf">Mex</span> of <span class="tex-span">{<i>c</i><sub class="lower-index">0</sub>, <i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index">10<sup class="upper-index">9</sup></sub>}</span>.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 100 000</span>)&nbsp;— the length of the array and the number of queries respectively.</p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers&nbsp;— <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines describes a single query.</p><p>The first type of query is described by three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>&nbsp;— the bounds of the subarray.</p><p>The second type of query is described by three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span> is the index of the element, which must be changed and <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> is the new value.</p>

## Output

<p>For each query of the first type output a single integer &nbsp;— the <span class="tex-font-style-bf">Mex</span> of <span class="tex-span">{<i>c</i><sub class="lower-index">0</sub>, <i>c</i><sub class="lower-index">1</sub>, ..., <i>c</i><sub class="lower-index">10<sup class="upper-index">9</sup></sub>}</span>.</p>





```input1
10 4
1 2 3 1 1 2 2 2 9 9
1 1 1
1 2 8
2 7 1
1 2 8

```




```output1
2
3
2

```



## Note

<p>The subarray of the first query consists of the single element&nbsp;— <span class="tex-span">1</span>. </p><p>The subarray of the second query consists of four <span class="tex-span">2</span>s, one <span class="tex-span">3</span> and two <span class="tex-span">1</span>s.</p><p>The subarray of the fourth query consists of three <span class="tex-span">1</span>s, three <span class="tex-span">2</span>s and one <span class="tex-span">3</span>.</p>
