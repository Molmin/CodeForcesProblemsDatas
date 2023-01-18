## Description

<div><p><span class="tex-font-style-it">Where do odds begin, and where do they end? Where does hope emerge, and will they ever break?</span></p><p>Given an integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> of length <span class="tex-span"><i>n</i></span>. Decide whether it is possible to divide it into an odd number of non-empty subsegments, the each of which has an odd length and begins and ends with odd numbers.</p><p>A <span class="tex-font-style-underline">subsegment</span> is a contiguous slice of the whole sequence. For example, <span class="tex-span">{3, 4, 5}</span> and <span class="tex-span">{1}</span> are subsegments of sequence <span class="tex-span">{1, 2, 3, 4, 5, 6}</span>, while <span class="tex-span">{1, 2, 4}</span> and <span class="tex-span">{7}</span> are not.</p></div><div class="input-specification"><p>The first line of input contains a non-negative integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the length of the sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of the sequence.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Yes</span>" if it's possible to fulfill the requirements, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of input contains a non-negative integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the length of the sequence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the elements of the sequence.</p>

## Output

<p>Output "<span class="tex-font-style-tt">Yes</span>" if it's possible to fulfill the requirements, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in any case (upper or lower).</p>





```input1
3
1 3 5

```




```input2
5
1 0 1 5 1

```




```input3
3
4 3 1

```




```input4
4
3 9 9 3

```




```output1
Yes

```




```output2
Yes

```




```output3
No

```




```output4
No

```



## Note

<p>In the first example, divide the sequence into <span class="tex-span">1</span> subsegment: <span class="tex-span">{1, 3, 5}</span> and the requirements will be met.</p><p>In the second example, divide the sequence into <span class="tex-span">3</span> subsegments: <span class="tex-span">{1, 0, 1}</span>, <span class="tex-span">{5}</span>, <span class="tex-span">{1}</span>.</p><p>In the third example, one of the subsegments must start with <span class="tex-span">4</span> which is an even number, thus the requirements cannot be met.</p><p>In the fourth example, the sequence can be divided into <span class="tex-span">2</span> subsegments: <span class="tex-span">{3, 9, 9}</span>, <span class="tex-span">{3}</span>, but this is not a valid solution because <span class="tex-span">2</span> is an even number.</p>
