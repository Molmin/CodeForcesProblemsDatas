## Description

<div><p>You are given an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> elements. The <span class="tex-font-style-it">imbalance value</span> of some subsegment of this array is the difference between the maximum and minimum element from this segment. The <span class="tex-font-style-it">imbalance value</span> of the array is the sum of <span class="tex-font-style-it">imbalance values</span> of all subsegments of this array.</p><p>For example, the <span class="tex-font-style-it">imbalance value</span> of array <span class="tex-span">[1, 4, 1]</span> is <span class="tex-span">9</span>, because there are <span class="tex-span">6</span> different subsegments of this array: </p><ul> <li> <span class="tex-span">[1]</span> (from index <span class="tex-span">1</span> to index <span class="tex-span">1</span>), <span class="tex-font-style-it">imbalance value</span> is <span class="tex-span">0</span>; </li><li> <span class="tex-span">[1, 4]</span> (from index <span class="tex-span">1</span> to index <span class="tex-span">2</span>), <span class="tex-font-style-it">imbalance value</span> is <span class="tex-span">3</span>; </li><li> <span class="tex-span">[1, 4, 1]</span> (from index <span class="tex-span">1</span> to index <span class="tex-span">3</span>), <span class="tex-font-style-it">imbalance value</span> is <span class="tex-span">3</span>; </li><li> <span class="tex-span">[4]</span> (from index <span class="tex-span">2</span> to index <span class="tex-span">2</span>), <span class="tex-font-style-it">imbalance value</span> is <span class="tex-span">0</span>; </li><li> <span class="tex-span">[4, 1]</span> (from index <span class="tex-span">2</span> to index <span class="tex-span">3</span>), <span class="tex-font-style-it">imbalance value</span> is <span class="tex-span">3</span>; </li><li> <span class="tex-span">[1]</span> (from index <span class="tex-span">3</span> to index <span class="tex-span">3</span>), <span class="tex-font-style-it">imbalance value</span> is <span class="tex-span">0</span>; </li></ul><p>You have to determine the <span class="tex-font-style-it">imbalance value</span> of the array <span class="tex-span"><i>a</i></span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — size of the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — elements of the array.</p></div><div class="output-specification"><p>Print one integer — the <span class="tex-font-style-it">imbalance value</span> of <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — size of the array <span class="tex-span"><i>a</i></span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — elements of the array.</p>

## Output

<p>Print one integer — the <span class="tex-font-style-it">imbalance value</span> of <span class="tex-span"><i>a</i></span>.</p>





```input1
3
1 4 1

```




```output1
9

```


