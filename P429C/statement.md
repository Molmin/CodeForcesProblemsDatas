## Description

<div><p>Iahub and Iahubina went to a picnic in a forest full of trees. Less than 5 minutes passed before Iahub remembered of trees from programming. Moreover, he invented a new problem and Iahubina has to solve it, otherwise Iahub won't give her the food. </p><p>Iahub asks Iahubina: can you build a rooted tree, such that</p><ul> <li> each internal node (a node with at least one son) has at least two sons; </li><li> node <span class="tex-span"><i>i</i></span> has <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> nodes in its subtree? </li></ul><p>Iahubina has to guess the tree. Being a smart girl, she realized that it's possible no tree can follow Iahub's restrictions. In this way, Iahub will eat all the food. You need to help Iahubina: determine if there's at least one tree following Iahub's restrictions. <span class="tex-font-style-bf">The required tree must contain <span class="tex-span"><i>n</i></span> nodes</span>.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>). Next line contains <span class="tex-span"><i>n</i></span> positive integers: the <span class="tex-span"><i>i</i></span>-th number represents <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>Output on the first line "<span class="tex-font-style-tt">YES</span>" (without quotes) if there exist at least one tree following Iahub's restrictions, otherwise output "<span class="tex-font-style-tt">NO</span>" (without quotes). </p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>). Next line contains <span class="tex-span"><i>n</i></span> positive integers: the <span class="tex-span"><i>i</i></span>-th number represents <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>Output on the first line "<span class="tex-font-style-tt">YES</span>" (without quotes) if there exist at least one tree following Iahub's restrictions, otherwise output "<span class="tex-font-style-tt">NO</span>" (without quotes). </p>





```input1
4
1 1 1 4

```




```input2
5
1 1 5 2 1

```




```output1
YES
```




```output2
NO
```


