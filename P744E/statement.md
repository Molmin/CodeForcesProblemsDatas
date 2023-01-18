## Description

<div><p>Hongcow's teacher heard that Hongcow had learned about the cyclic shift, and decided to set the following problem for him.</p><p>You are given a list of <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> contained in the list <span class="tex-span"><i>A</i></span>.</p><p>A list <span class="tex-span"><i>X</i></span> of strings is called <span class="tex-font-style-it">stable</span> if the following condition holds.</p><p>First, a <span class="tex-font-style-it">message</span> is defined as a concatenation of some elements of the list <span class="tex-span"><i>X</i></span>. You can use an arbitrary element as many times as you want, and you may concatenate these elements in any arbitrary order. Let <span class="tex-span"><i>S</i><sub class="lower-index"><i>X</i></sub></span> denote the set of of all messages you can construct from the list. Of course, this set has infinite size if your list is nonempty.</p><p>Call a single message <span class="tex-font-style-it">good</span> if the following conditions hold: </p><ul> <li> Suppose the message is the concatenation of <span class="tex-span"><i>k</i></span> strings <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>k</i></sub></span>, where each <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> is an element of <span class="tex-span"><i>X</i></span>. </li><li> Consider the <span class="tex-span">|<i>w</i><sub class="lower-index">1</sub>| + |<i>w</i><sub class="lower-index">2</sub>| + ... + |<i>w</i><sub class="lower-index"><i>k</i></sub>|</span> cyclic shifts of the string. Let <span class="tex-span"><i>m</i></span> be the number of these cyclic shifts of the string that are elements of <span class="tex-span"><i>S</i><sub class="lower-index"><i>X</i></sub></span>. </li><li> A message is good if and only if <span class="tex-span"><i>m</i></span> is exactly equal to <span class="tex-span"><i>k</i></span>. </li></ul><p>The list <span class="tex-span"><i>X</i></span> is called stable if and only if every element of <span class="tex-span"><i>S</i><sub class="lower-index"><i>X</i></sub></span> is good.</p><p>Let <span class="tex-span"><i>f</i>(<i>L</i>)</span> be <span class="tex-span">1</span> if <span class="tex-span"><i>L</i></span> is a stable list, and <span class="tex-span">0</span> otherwise.</p><p>Find the sum of <span class="tex-span"><i>f</i>(<i>L</i>)</span> where <span class="tex-span"><i>L</i></span> is a nonempty <span class="tex-font-style-bf">contiguous sublist</span> of <span class="tex-span"><i>A</i></span> (there are <img align="middle" class="tex-formula" src="file://j115rqGs.png" style="max-width: 100.0%;max-height: 100.0%;"> contiguous sublists in total).</p></div><div class="input-specification"><p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>), denoting the number of strings in the list.</p><p>The next <span class="tex-span"><i>n</i></span> lines will each contain a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://b8GLbGEk.png" style="max-width: 100.0%;max-height: 100.0%;">).</p></div><div class="output-specification"><p>Print a single integer, the number of nonempty <span class="tex-font-style-bf">contiguous sublists</span> that are stable.</p></div>

## Input

<p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30</span>), denoting the number of strings in the list.</p><p>The next <span class="tex-span"><i>n</i></span> lines will each contain a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://b8GLbGEk.png" style="max-width: 100.0%;max-height: 100.0%;">).</p>

## Output

<p>Print a single integer, the number of nonempty <span class="tex-font-style-bf">contiguous sublists</span> that are stable.</p>





```input1
4
a
ab
b
bba

```




```input2
5
hh
ee
ll
ll
oo

```




```input3
6
aab
ab
bba
b
ab
c

```




```output1
7

```




```output2
0

```




```output3
13

```



## Note

<p>For the first sample, there are <span class="tex-span">10</span> sublists to consider. Sublists ["<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">b</span>"], ["<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">bba</span>"], and ["<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">bba</span>"] are not stable. The other seven sublists are stable.</p><p>For example, <span class="tex-span"><i>X</i></span> = ["<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">b</span>"] is not stable, since the message "<span class="tex-font-style-tt">ab</span>" + "<span class="tex-font-style-tt">ab</span>" = "<span class="tex-font-style-tt">abab</span>" has four cyclic shifts ["<span class="tex-font-style-tt">abab</span>", "<span class="tex-font-style-tt">baba</span>", "<span class="tex-font-style-tt">abab</span>", "<span class="tex-font-style-tt">baba</span>"], which are all elements of <span class="tex-span"><i>S</i><sub class="lower-index"><i>X</i></sub></span>.</p>
