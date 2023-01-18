## Description

<div><p>Vasya likes everything infinite. Now he is studying the properties of a sequence <span class="tex-span"><i>s</i></span>, such that its first element is equal to <span class="tex-span"><i>a</i></span> (<span class="tex-span"><i>s</i><sub class="lower-index">1</sub> = <i>a</i></span>), and the difference between any two neighbouring elements is equal to <span class="tex-span"><i>c</i></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> - <i>s</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>c</i></span>). In particular, Vasya wonders if his favourite integer <span class="tex-span"><i>b</i></span> appears in this sequence, that is, there exists a positive integer <span class="tex-span"><i>i</i></span>, such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>b</i></span>. Of course, you are the person he asks for a help.</p></div><div class="input-specification"><p>The first line of the input contain three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the first element of the sequence, Vasya's favorite number and the difference between any two neighbouring elements of the sequence, respectively.</p></div><div class="output-specification"><p>If <span class="tex-span"><i>b</i></span> appears in the sequence <span class="tex-span"><i>s</i></span> print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contain three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the first element of the sequence, Vasya's favorite number and the difference between any two neighbouring elements of the sequence, respectively.</p>

## Output

<p>If <span class="tex-span"><i>b</i></span> appears in the sequence <span class="tex-span"><i>s</i></span> print "<span class="tex-font-style-tt">YES</span>" (without quotes), otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
1 7 3

```




```input2
10 10 0

```




```input3
1 -4 5

```




```input4
0 60 50

```




```output1
YES

```




```output2
YES

```




```output3
NO

```




```output4
NO

```



## Note

<p>In the first sample, the sequence starts from integers <span class="tex-span">1</span>, <span class="tex-span">4</span>, <span class="tex-span">7</span>, so <span class="tex-span">7</span> is its element.</p><p>In the second sample, the favorite integer of Vasya is equal to the first element of the sequence.</p><p>In the third sample all elements of the sequence are greater than Vasya's favorite integer.</p><p>In the fourth sample, the sequence starts from <span class="tex-span">0</span>, <span class="tex-span">50</span>, <span class="tex-span">100</span>, and all the following elements are greater than Vasya's favorite integer.</p>
