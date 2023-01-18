## Description

<div><p>The organizers of a programming contest have decided to present t-shirts to participants. There are six different t-shirts sizes in this problem: <span class="tex-font-style-tt">S</span>, <span class="tex-font-style-tt">M</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">XL</span>, <span class="tex-font-style-tt">XXL</span>, <span class="tex-font-style-tt">XXXL</span> (sizes are listed in increasing order). The t-shirts are already prepared. For each size from <span class="tex-font-style-tt">S</span> to <span class="tex-font-style-tt">XXXL</span> you are given the number of t-shirts of this size.</p><p>During the registration, the organizers asked each of the <span class="tex-span"><i>n</i></span> participants about the t-shirt size he wants. If a participant hesitated between two sizes, he could specify two neighboring sizes&nbsp;— this means that any of these two sizes suits him.</p><p>Write a program that will determine whether it is possible to present a t-shirt to each participant of the competition, or not. Of course, each participant should get a t-shirt of proper size: </p><ul> <li> the size he wanted, if he specified one size; </li><li> any of the two neibouring sizes, if he specified two sizes. </li></ul><p>If it is possible, the program should find any valid distribution of the t-shirts.</p></div><div class="input-specification"><p>The first line of the input contains six non-negative integers&nbsp;— the number of t-shirts of each size. The numbers are given for the sizes <span class="tex-font-style-tt">S</span>, <span class="tex-font-style-tt">M</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">XL</span>, <span class="tex-font-style-tt">XXL</span>, <span class="tex-font-style-tt">XXXL</span>, respectively. The total number of t-shirts doesn't exceed <span class="tex-span">100 000</span>.</p><p>The second line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of participants.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain the sizes specified by the participants, one line per participant. The <span class="tex-span"><i>i</i></span>-th line contains information provided by the <span class="tex-span"><i>i</i></span>-th participant: single size or two sizes separated by comma (without any spaces). If there are two sizes, the sizes are written in increasing order. It is guaranteed that two sizes separated by comma are neighboring.</p></div><div class="output-specification"><p>If it is not possible to present a t-shirt to each participant, print «<span class="tex-font-style-tt">NO</span>» (without quotes).</p><p>Otherwise, print <span class="tex-span"><i>n</i> + 1</span> lines. In the first line print «<span class="tex-font-style-tt">YES</span>» (without quotes). In the following <span class="tex-span"><i>n</i></span> lines print the t-shirt sizes the orginizers should give to participants, one per line. The order of the participants should be the same as in the input.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line of the input contains six non-negative integers&nbsp;— the number of t-shirts of each size. The numbers are given for the sizes <span class="tex-font-style-tt">S</span>, <span class="tex-font-style-tt">M</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">XL</span>, <span class="tex-font-style-tt">XXL</span>, <span class="tex-font-style-tt">XXXL</span>, respectively. The total number of t-shirts doesn't exceed <span class="tex-span">100 000</span>.</p><p>The second line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of participants.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain the sizes specified by the participants, one line per participant. The <span class="tex-span"><i>i</i></span>-th line contains information provided by the <span class="tex-span"><i>i</i></span>-th participant: single size or two sizes separated by comma (without any spaces). If there are two sizes, the sizes are written in increasing order. It is guaranteed that two sizes separated by comma are neighboring.</p>

## Output

<p>If it is not possible to present a t-shirt to each participant, print «<span class="tex-font-style-tt">NO</span>» (without quotes).</p><p>Otherwise, print <span class="tex-span"><i>n</i> + 1</span> lines. In the first line print «<span class="tex-font-style-tt">YES</span>» (without quotes). In the following <span class="tex-span"><i>n</i></span> lines print the t-shirt sizes the orginizers should give to participants, one per line. The order of the participants should be the same as in the input.</p><p>If there are multiple solutions, print any of them.</p>





```input1
0 1 0 1 1 0
3
XL
S,M
XL,XXL

```




```input2
1 1 2 0 1 1
5
S
M
S,M
XXL,XXXL
XL,XXL

```




```output1
YES
XL
M
XXL

```




```output2
NO

```


