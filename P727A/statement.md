## Description

<div><p>Vasily has a number <span class="tex-span"><i>a</i></span>, which he wants to turn into a number <span class="tex-span"><i>b</i></span>. For this purpose, he can do two types of operations:</p><ul> <li> multiply the current number by <span class="tex-span">2</span> (that is, replace the number <span class="tex-span"><i>x</i></span> by <span class="tex-span">2·<i>x</i></span>); </li><li> append the digit <span class="tex-span">1</span> to the right of current number (that is, replace the number <span class="tex-span"><i>x</i></span> by <span class="tex-span">10·<i>x</i> + 1</span>). </li></ul><p>You need to help Vasily to transform the number <span class="tex-span"><i>a</i></span> into the number <span class="tex-span"><i>b</i></span> using only the operations described above, or find that it is impossible.</p><p>Note that in this task you are not required to minimize the number of operations. It suffices to find any way to transform <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number which Vasily has and the number he wants to have.</p></div><div class="output-specification"><p>If there is no way to get <span class="tex-span"><i>b</i></span> from <span class="tex-span"><i>a</i></span>, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print three lines. On the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes). The second line should contain single integer <span class="tex-span"><i>k</i></span>&nbsp;— the length of the transformation sequence. On the third line print the sequence of transformations <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span>, where:</p><ul> <li> <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> should be equal to <span class="tex-span"><i>a</i></span>, </li><li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> should be equal to <span class="tex-span"><i>b</i></span>, </li><li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> should be obtained from <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i> - 1</sub></span> using any of two described operations (<span class="tex-span">1 &lt; <i>i</i> ≤ <i>k</i></span>). </li></ul><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> &lt; <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number which Vasily has and the number he wants to have.</p>

## Output

<p>If there is no way to get <span class="tex-span"><i>b</i></span> from <span class="tex-span"><i>a</i></span>, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise print three lines. On the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes). The second line should contain single integer <span class="tex-span"><i>k</i></span>&nbsp;— the length of the transformation sequence. On the third line print the sequence of transformations <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span>, where:</p><ul> <li> <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> should be equal to <span class="tex-span"><i>a</i></span>, </li><li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>k</i></sub></span> should be equal to <span class="tex-span"><i>b</i></span>, </li><li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> should be obtained from <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i> - 1</sub></span> using any of two described operations (<span class="tex-span">1 &lt; <i>i</i> ≤ <i>k</i></span>). </li></ul><p>If there are multiple answers, print any of them.</p>





```input1
2 162

```




```input2
4 42

```




```input3
100 40021

```




```output1
YES
5
2 4 8 81 162 

```




```output2
NO

```




```output3
YES
5
100 200 2001 4002 40021 

```


