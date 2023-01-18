## Description

<div><p>Recently Ivan noticed an array <span class="tex-span"><i>a</i></span> while debugging his code. Now Ivan can't remember this array, but the bug he was trying to fix didn't go away, so Ivan thinks that the data from this array might help him to reproduce the bug.</p><p>Ivan clearly remembers that there were <span class="tex-span"><i>n</i></span> elements in the array, and each element was not less than <span class="tex-span">1</span> and not greater than <span class="tex-span"><i>n</i></span>. Also he remembers <span class="tex-span"><i>q</i></span> facts about the array. There are two types of facts that Ivan remembers:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> — for each <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub> ≥ <i>v</i><sub class="lower-index"><i>i</i></sub></span>; </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> — for each <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>x</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>x</i></sub> ≤ <i>v</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul><p>Also Ivan thinks that this array was a permutation, but he is not so sure about it. He wants to restore some array that corresponds to the <span class="tex-span"><i>q</i></span> facts that he remembers and is very similar to permutation. Formally, Ivan has denoted the <span class="tex-span"><i>cost</i></span> of array as follows:</p><p><img align="middle" class="tex-formula" src="file://71ZaMT5R.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>cnt</i>(<i>i</i>)</span> is the number of occurences of <span class="tex-span"><i>i</i></span> in the array.</p><p>Help Ivan to determine minimum possible <span class="tex-span"><i>cost</i></span> of the array that corresponds to the facts!</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 100</span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each representing a fact about the array. <span class="tex-span"><i>i</i></span>-th line contains the numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span"><i>i</i></span>-th fact (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the type of the fact).</p></div><div class="output-specification"><p>If the facts are controversial and there is no array that corresponds to them, print <span class="tex-font-style-tt">-1</span>. Otherwise, print minimum possible <span class="tex-span"><i>cost</i></span> of the array.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 100</span>).</p><p>Then <span class="tex-span"><i>q</i></span> lines follow, each representing a fact about the array. <span class="tex-span"><i>i</i></span>-th line contains the numbers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span"><i>i</i></span>-th fact (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the type of the fact).</p>

## Output

<p>If the facts are controversial and there is no array that corresponds to them, print <span class="tex-font-style-tt">-1</span>. Otherwise, print minimum possible <span class="tex-span"><i>cost</i></span> of the array.</p>





```input1
3 0

```




```input2
3 1
1 1 3 2

```




```input3
3 2
1 1 3 2
2 1 3 2

```




```input4
3 2
1 1 3 2
2 1 3 1

```




```output1
3

```




```output2
5

```




```output3
9

```




```output4
-1

```


