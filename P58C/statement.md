## Description

<div><p>On Bertown's main street <span class="tex-span"><i>n</i></span> trees are growing, the tree number <span class="tex-span"><i>i</i></span> has the height of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> meters (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). By the arrival of the President of Berland these trees were decided to be changed so that their heights formed a <span class="tex-font-style-underline">beautiful</span> sequence. This means that the heights of trees on ends (the <span class="tex-span">1</span>st one and the <span class="tex-span"><i>n</i></span>-th one) should be equal to each other, the heights of the <span class="tex-span">2</span>-nd and the <span class="tex-span">(<i>n</i> - 1)</span>-th tree must also be equal to each other, at that the height of the <span class="tex-span">2</span>-nd tree should be larger than the height of the first tree by <span class="tex-span">1</span>, and so on. In other words, the heights of the trees, standing at equal distance from the edge (of one end of the sequence) must be equal to each other, and with the increasing of the distance from the edge by <span class="tex-span">1</span> the tree height must also increase by <span class="tex-span">1</span>. For example, the sequences "<span class="tex-font-style-tt">2 3 4 5 5 4 3 2</span>" and "<span class="tex-font-style-tt">1 2 3 2 1</span>" are beautiful, and '<span class="tex-font-style-tt">1 3 3 1</span>" and "<span class="tex-font-style-tt">1 2 3 1</span>" are not. </p><p>Changing the height of a tree is a very expensive operation, using advanced technologies invented by Berland scientists. In one operation you can choose any tree and change its height to any number, either increase or decrease. Note that even after the change the height should remain a positive integer, i. e, it can't be less than or equal to zero. Identify the smallest number of changes of the trees' height needed for the sequence of their heights to become beautiful.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which is the number of trees. The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) which are the heights of the trees.</p></div><div class="output-specification"><p>Print a single number which is the minimal number of trees whose heights will have to be changed for the sequence to become beautiful.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which is the number of trees. The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) which are the heights of the trees.</p>

## Output

<p>Print a single number which is the minimal number of trees whose heights will have to be changed for the sequence to become beautiful.</p>





```input1
3
2 2 2

```




```input2
4
1 2 2 1

```




```output1
1

```




```output2
0

```


