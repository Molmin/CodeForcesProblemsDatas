## Description

<div><p>A simple recommendation system would recommend a user things liked by a certain number of their friends. In this problem you will implement part of such a system.</p><p>You are given user's friends' opinions about a list of items. You are also given a threshold <span class="tex-span"><i>T</i></span> — the minimal number of "likes" necessary for an item to be recommended to the user.</p><p>Output the number of items in the list liked by at least <span class="tex-span"><i>T</i></span> of user's friends.</p></div><div class="input-specification"><p>The first line of the input will contain three space-separated integers: the number of friends <span class="tex-span"><i>F</i></span> (<span class="tex-span">1 ≤ <i>F</i> ≤ 10</span>), the number of items <span class="tex-span"><i>I</i></span> (<span class="tex-span">1 ≤ <i>I</i> ≤ 10</span>) and the threshold <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ <i>F</i></span>).</p><p>The following <span class="tex-span"><i>F</i></span> lines of input contain user's friends' opinions. <span class="tex-span"><i>j</i></span>-th character of <span class="tex-span"><i>i</i></span>-th line is '<span class="tex-font-style-tt">Y</span>' if <span class="tex-span"><i>i</i></span>-th friend likes <span class="tex-span"><i>j</i></span>-th item, and '<span class="tex-font-style-tt">N</span>' otherwise.</p></div><div class="output-specification"><p>Output an integer — the number of items liked by at least <span class="tex-span"><i>T</i></span> of user's friends.</p></div>

## Input

<p>The first line of the input will contain three space-separated integers: the number of friends <span class="tex-span"><i>F</i></span> (<span class="tex-span">1 ≤ <i>F</i> ≤ 10</span>), the number of items <span class="tex-span"><i>I</i></span> (<span class="tex-span">1 ≤ <i>I</i> ≤ 10</span>) and the threshold <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ <i>F</i></span>).</p><p>The following <span class="tex-span"><i>F</i></span> lines of input contain user's friends' opinions. <span class="tex-span"><i>j</i></span>-th character of <span class="tex-span"><i>i</i></span>-th line is '<span class="tex-font-style-tt">Y</span>' if <span class="tex-span"><i>i</i></span>-th friend likes <span class="tex-span"><i>j</i></span>-th item, and '<span class="tex-font-style-tt">N</span>' otherwise.</p>

## Output

<p>Output an integer — the number of items liked by at least <span class="tex-span"><i>T</i></span> of user's friends.</p>





```input1
3 3 2
YYY
NNN
YNY

```




```input2
4 4 1
NNNY
NNYN
NYNN
YNNN

```




```output1
2

```




```output2
4

```


