## Description

<div><p>Once upon a time in the thicket of the mushroom forest lived mushroom gnomes. They were famous among their neighbors for their magic mushrooms. Their magic nature made it possible that between every two neighboring mushrooms every minute grew another mushroom with the weight equal to the sum of weights of two neighboring ones. </p><p>The mushroom gnomes loved it when everything was in order, that's why they always planted the mushrooms in one line in the order of their weights' increasing. Well... The gnomes planted the mushrooms and went to eat. After <span class="tex-span"><i>x</i></span> minutes they returned and saw that new mushrooms had grown up, so that the increasing order had been violated. The gnomes replanted all the mushrooms in the correct order, that is, they sorted the mushrooms in the order of the weights' increasing. And went to eat again (those gnomes were quite big eaters). What total weights modulo <span class="tex-span"><i>p</i></span> will the mushrooms have in another <span class="tex-span"><i>y</i></span> minutes?</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">18</sup>, <i>x</i> + <i>y</i> &gt; 0, 2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>) which represent the number of mushrooms, the number of minutes after the first replanting, the number of minutes after the second replanting and the module. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> which represent the mushrooms' weight in the non-decreasing order (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div><div class="output-specification"><p>The answer should contain a single number which is the total weights of the mushrooms modulo <span class="tex-span"><i>p</i></span> in the end after <span class="tex-span"><i>x</i> + <i>y</i></span> minutes.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup>, 0 ≤ <i>x</i>, <i>y</i> ≤ 10<sup class="upper-index">18</sup>, <i>x</i> + <i>y</i> &gt; 0, 2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>) which represent the number of mushrooms, the number of minutes after the first replanting, the number of minutes after the second replanting and the module. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> which represent the mushrooms' weight in the non-decreasing order (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cin</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>

## Output

<p>The answer should contain a single number which is the total weights of the mushrooms modulo <span class="tex-span"><i>p</i></span> in the end after <span class="tex-span"><i>x</i> + <i>y</i></span> minutes.</p>





```input1
2 1 0 657276545
1 2

```




```input2
2 1 1 888450282
1 2

```




```input3
4 5 0 10000
1 2 3 4

```




```output1
6

```




```output2
14

```




```output3
1825

```


