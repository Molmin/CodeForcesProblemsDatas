## Description

<div><p>Yesterday was a fair in a supermarket's grocery section. There were <span class="tex-span"><i>n</i></span> jars with spices on the fair. Before the event the jars were numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the left to the right. After the event the jars were moved and the grocer had to sort them by the increasing of the numbers.</p><p>The grocer has a special machine at his disposal. The machine can take any <span class="tex-span">5</span> or less jars and rearrange them in the way the grocer wants. Note that the jars <span class="tex-font-style-bf">do not have to</span> stand consecutively. For example, from the permutation <span class="tex-span">2</span>, <span class="tex-span">6</span>, <span class="tex-span">5</span>, <span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">1</span> one can get permutation <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span>, <span class="tex-span">6</span>, if pick the jars on the positions <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span>. </p><p>Which minimum number of such operations is needed to arrange all the jars in the order of their numbers' increasing?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the <span class="tex-span"><i>i</i></span>-th number represents the number of a jar that occupies the <span class="tex-span"><i>i</i></span>-th position. It is guaranteed that all the numbers are distinct.</p></div><div class="output-specification"><p>Print on the first line the least number of operations needed to rearrange all the jars in the order of the numbers' increasing. Then print the description of all actions in the following format.</p><p>On the first line of the description of one action indicate the number of jars that need to be taken (<span class="tex-span"><i>k</i></span>), on the second line indicate from which positions the jars need to be taken (<span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span>), on the third line indicate the jar's new order (<span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span>). After the operation is fulfilled the jar from position <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will occupy the position <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The set (<span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span>) should be the rearrangement of the set (<span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span>).</p><p>If there are multiple solutions, output any.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the <span class="tex-span"><i>i</i></span>-th number represents the number of a jar that occupies the <span class="tex-span"><i>i</i></span>-th position. It is guaranteed that all the numbers are distinct.</p>

## Output

<p>Print on the first line the least number of operations needed to rearrange all the jars in the order of the numbers' increasing. Then print the description of all actions in the following format.</p><p>On the first line of the description of one action indicate the number of jars that need to be taken (<span class="tex-span"><i>k</i></span>), on the second line indicate from which positions the jars need to be taken (<span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span>), on the third line indicate the jar's new order (<span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span>). After the operation is fulfilled the jar from position <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will occupy the position <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The set (<span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span>) should be the rearrangement of the set (<span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span>).</p><p>If there are multiple solutions, output any.</p>





```input1
6
3 5 6 1 2 4

```




```input2
14
9 13 11 3 10 7 12 14 1 5 4 6 8 2

```




```output1
2
4
1 3 6 4 
3 6 4 1 
2
2 5 
5 2 

```




```output2
3
4
2 13 8 14 
13 8 14 2 
5
6 7 12 5 10 
7 12 6 10 5 
5
3 11 4 1 9 
11 4 3 9 1 

```



## Note

<p>Let's consider the first sample. The jars can be sorted within two actions.</p><p>During the first action we take the jars from positions <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">6</span> and <span class="tex-span">4</span> and put them so that the jar that used to occupy the position <span class="tex-span">1</span> will occupy the position <span class="tex-span">3</span> after the operation is completed. The jar from position <span class="tex-span">3</span> will end up in position <span class="tex-span">6</span>, the jar from position <span class="tex-span">6</span> will end up in position <span class="tex-span">4</span> and the jar from position <span class="tex-span">4</span> will end up in position <span class="tex-span">1</span>.</p><p>After the first action the order will look like that: <span class="tex-span">1</span>, <span class="tex-span">5</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">2</span>, <span class="tex-span">6</span>. </p><p>During the second operation the jars in positions <span class="tex-span">2</span> and <span class="tex-span">5</span> will change places.</p>
