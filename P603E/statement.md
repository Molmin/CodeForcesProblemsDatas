## Description

<div><p>In the land of Bovinia there are <span class="tex-span"><i>n</i></span> pastures, but no paths connecting the pastures. Of course, this is a terrible situation, so Kevin Sun is planning to rectify it by constructing <span class="tex-span"><i>m</i></span> undirected paths connecting pairs of distinct pastures. To make transportation more efficient, he also plans to pave some of these new paths.</p><p>Kevin is very particular about certain aspects of path-paving. Since he loves odd numbers, he wants each pasture to have an odd number of paved paths connected to it. Thus we call a paving <span class="tex-font-style-underline">sunny</span> if each pasture is incident to an odd number of paved paths. He also enjoys short paths more than long paths, so he would like the longest paved path to be as short as possible. After adding each path, Kevin wants to know if a sunny paving exists for the paths of Bovinia, and if at least one does, the minimum possible length of the longest path in such a paving. Note that "longest path" here means maximum-weight edge.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 300 000</span>), denoting the number of pastures and paths, respectively. The next <span class="tex-span"><i>m</i></span> lines each contain three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, describing the <span class="tex-span"><i>i</i></span>-th path. The <span class="tex-span"><i>i</i></span>-th path connects pastures <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) and has length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Paths are given in the order in which they are constructed. </p></div><div class="output-specification"><p>Output <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain a single integer denoting the minimum possible length of the longest path (maximum-weight edge) in a sunny paving using only the first <span class="tex-span"><i>i</i></span> paths. If Kevin cannot pave a set of paths so that each pasture is incident to an odd number of paved paths, output <span class="tex-span"> - 1</span>.</p><p>Note that the paving is only hypothetical—your answer after adding the <span class="tex-span"><i>i</i></span>-th path should not be affected by any of your previous answers.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 300 000</span>), denoting the number of pastures and paths, respectively. The next <span class="tex-span"><i>m</i></span> lines each contain three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, describing the <span class="tex-span"><i>i</i></span>-th path. The <span class="tex-span"><i>i</i></span>-th path connects pastures <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) and has length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). Paths are given in the order in which they are constructed. </p>

## Output

<p>Output <span class="tex-span"><i>m</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain a single integer denoting the minimum possible length of the longest path (maximum-weight edge) in a sunny paving using only the first <span class="tex-span"><i>i</i></span> paths. If Kevin cannot pave a set of paths so that each pasture is incident to an odd number of paved paths, output <span class="tex-span"> - 1</span>.</p><p>Note that the paving is only hypothetical—your answer after adding the <span class="tex-span"><i>i</i></span>-th path should not be affected by any of your previous answers.</p>





```input1
4 4
1 3 4
2 4 8
1 2 2
3 4 3

```




```input2
3 2
1 2 3
2 3 4

```




```input3
4 10
2 1 987
3 2 829
4 1 768
4 2 608
3 4 593
3 2 488
4 2 334
2 1 204
1 3 114
1 4 39

```




```output1
-1
8
8
3

```




```output2
-1
-1

```




```output3
-1
-1
829
829
768
768
768
488
334
204

```



## Note

<p>For the first sample, these are the paths that Kevin should pave after building the <span class="tex-span"><i>i</i></span>-th path: </p><ol> <li> No set of paths works. </li><li> Paths 1 (length <span class="tex-span">4</span>) and 2 (length <span class="tex-span">8</span>). </li><li> Paths 1 (length <span class="tex-span">4</span>) and 2 (length <span class="tex-span">8</span>). </li><li> Paths 3 (length <span class="tex-span">2</span>) and 4 (length <span class="tex-span">3</span>). </li></ol><p>In the second sample, there never exists a paving that makes Kevin happy.</p>
