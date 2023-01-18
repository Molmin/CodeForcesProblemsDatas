## Description

<div><p>Valera's finally decided to go on holiday! He packed up and headed for a ski resort.</p><p>Valera's fancied a ski trip but he soon realized that he could get lost in this new place. Somebody gave him a useful hint: the resort has <span class="tex-span"><i>n</i></span> objects (we will consider the objects indexed in some way by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>), each object is either a hotel or a mountain.</p><p>Valera has also found out that the ski resort had multiple ski tracks. Specifically, for each object <span class="tex-span"><i>v</i></span>, the resort has at most one object <span class="tex-span"><i>u</i></span>, such that there is a ski track built from object <span class="tex-span"><i>u</i></span> to object <span class="tex-span"><i>v</i></span>. We also know that no hotel has got a ski track leading from the hotel to some object.</p><p>Valera is afraid of getting lost on the resort. So he wants you to come up with a path he would walk along. The path must consist of objects <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span"><i>k</i> ≥ 1</span>) and meet the following conditions:</p><ol> <li> Objects with numbers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i> - 1</sub></span> are mountains and the object with number <span class="tex-span"><i>v</i><sub class="lower-index"><i>k</i></sub></span> is the hotel. </li><li> For any integer <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>k</i>)</span>, there is <span class="tex-font-style-bf">exactly one</span> ski track leading from object <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. This track goes to object <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span>. </li><li> The path contains as many objects as possible (<span class="tex-span"><i>k</i></span> is maximal). </li></ol><p>Help Valera. Find such path that meets all the criteria of our hero!</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of objects.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>type</i><sub class="lower-index">1</sub>, <i>type</i><sub class="lower-index">2</sub>, ..., <i>type</i><sub class="lower-index"><i>n</i></sub></span> — the types of the objects. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> equals zero, then the <span class="tex-span"><i>i</i></span>-th object is the mountain. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> equals one, then the <span class="tex-span"><i>i</i></span>-th object is the hotel. It is guaranteed that at least one object is a hotel.</p><p>The third line of the input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the description of the ski tracks. If number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals zero, then there is no such object <span class="tex-span"><i>v</i></span>, that has a ski track built from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>i</i></span>. If number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> doesn't equal zero, that means that there is a track built from object <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to object <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>k</i></span> — the maximum possible path length for Valera. In the second line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i></sub></span> — the path. If there are multiple solutions, you can print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of objects.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>type</i><sub class="lower-index">1</sub>, <i>type</i><sub class="lower-index">2</sub>, ..., <i>type</i><sub class="lower-index"><i>n</i></sub></span> — the types of the objects. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> equals zero, then the <span class="tex-span"><i>i</i></span>-th object is the mountain. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> equals one, then the <span class="tex-span"><i>i</i></span>-th object is the hotel. It is guaranteed that at least one object is a hotel.</p><p>The third line of the input contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the description of the ski tracks. If number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals zero, then there is no such object <span class="tex-span"><i>v</i></span>, that has a ski track built from <span class="tex-span"><i>v</i></span> to <span class="tex-span"><i>i</i></span>. If number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> doesn't equal zero, that means that there is a track built from object <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to object <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>In the first line print <span class="tex-span"><i>k</i></span> — the maximum possible path length for Valera. In the second line print <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>k</i></sub></span> — the path. If there are multiple solutions, you can print any of them.</p>





```input1
5
0 0 0 0 1
0 1 2 3 4

```




```input2
5
0 0 1 0 1
0 1 2 2 4

```




```input3
4
1 0 0 0
2 3 4 2

```




```output1
5
1 2 3 4 5

```




```output2
2
4 5

```




```output3
1
1

```


