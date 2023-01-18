## Description

<div><p>Limak is a little polar bear. Polar bears hate long strings and thus they like to compress them. You should also know that Limak is so young that he knows only first six letters of the English alphabet: '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">d</span>', '<span class="tex-font-style-tt">e</span>' and '<span class="tex-font-style-tt">f</span>'.</p><p>You are given a set of <span class="tex-span"><i>q</i></span> possible operations. Limak can perform them in any order, any operation may be applied any number of times. The <span class="tex-span"><i>i</i></span>-th operation is described by a string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of length two and a string <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of length one. No two of <span class="tex-span"><i>q</i></span> possible operations have the same string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>When Limak has a string <span class="tex-span"><i>s</i></span> he can perform the <span class="tex-span"><i>i</i></span>-th operation on <span class="tex-span"><i>s</i></span> if the first two letters of <span class="tex-span"><i>s</i></span> match a two-letter string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Performing the <span class="tex-span"><i>i</i></span>-th operation removes first two letters of <span class="tex-span"><i>s</i></span> and inserts there a string <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. See the notes section for further clarification.</p><p>You may note that performing an operation decreases the length of a string <span class="tex-span"><i>s</i></span> exactly by <span class="tex-span">1</span>. Also, for some sets of operations there may be a string that cannot be compressed any further, because the first two letters don't match any <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Limak wants to start with a string of length <span class="tex-span"><i>n</i></span> and perform <span class="tex-span"><i>n</i> - 1</span> operations to finally get a one-letter string "<span class="tex-font-style-tt">a</span>". In how many ways can he choose the starting string to be able to get "<span class="tex-font-style-tt">a</span>"? Remember that Limak can use only letters he knows.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 6</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 36</span>)&nbsp;— the length of the initial string and the number of available operations.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the possible operations. The <span class="tex-span"><i>i</i></span>-th of them contains two strings <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| = 2, |<i>b</i><sub class="lower-index"><i>i</i></sub>| = 1</span>). It's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> for <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> consist of only first six lowercase English letters.</p></div><div class="output-specification"><p>Print the number of strings of length <span class="tex-span"><i>n</i></span> that Limak will be able to transform to string "<span class="tex-font-style-tt">a</span>" by applying only operations given in the input.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 6</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 36</span>)&nbsp;— the length of the initial string and the number of available operations.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the possible operations. The <span class="tex-span"><i>i</i></span>-th of them contains two strings <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| = 2, |<i>b</i><sub class="lower-index"><i>i</i></sub>| = 1</span>). It's guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>a</i><sub class="lower-index"><i>j</i></sub></span> for <span class="tex-span"><i>i</i> ≠ <i>j</i></span> and that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> consist of only first six lowercase English letters.</p>

## Output

<p>Print the number of strings of length <span class="tex-span"><i>n</i></span> that Limak will be able to transform to string "<span class="tex-font-style-tt">a</span>" by applying only operations given in the input.</p>





```input1
3 5
ab a
cc c
ca a
ee c
ff d

```




```input2
2 8
af e
dc d
cc f
bc b
da b
eb a
bb b
ff c

```




```input3
6 2
bb a
ba a

```




```output1
4

```




```output2
1

```




```output3
0

```



## Note

<p>In the first sample, we count initial strings of length <span class="tex-span">3</span> from which Limak can get a required string "<span class="tex-font-style-tt">a</span>". There are <span class="tex-span">4</span> such strings: "<span class="tex-font-style-tt">abb</span>", "<span class="tex-font-style-tt">cab</span>", "<span class="tex-font-style-tt">cca</span>", "<span class="tex-font-style-tt">eea</span>". The first one Limak can compress using operation <span class="tex-span">1</span> two times (changing "<span class="tex-font-style-tt">ab</span>" to a single "<span class="tex-font-style-tt">a</span>"). The first operation would change "<span class="tex-font-style-tt">abb</span>" to "<span class="tex-font-style-tt">ab</span>" and the second operation would change "<span class="tex-font-style-tt">ab</span>" to "<span class="tex-font-style-tt">a</span>".</p><p>Other three strings may be compressed as follows: </p><ul> <li> "<span class="tex-font-style-tt">cab</span>" <img align="middle" class="tex-formula" src="file://3P8ztuBh.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">ab</span>" <img align="middle" class="tex-formula" src="file://CgUtEICl.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">a</span>" </li><li> "<span class="tex-font-style-tt">cca</span>" <img align="middle" class="tex-formula" src="file://TupRXuVc.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">ca</span>" <img align="middle" class="tex-formula" src="file://Y4A8eHnU.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">a</span>" </li><li> "<span class="tex-font-style-tt">eea</span>" <img align="middle" class="tex-formula" src="file://MhhogTpJ.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">ca</span>" <img align="middle" class="tex-formula" src="file://X0LW48Ci.png" style="max-width: 100.0%;max-height: 100.0%;"> "<span class="tex-font-style-tt">a</span>" </li></ul><p>In the second sample, the only correct initial string is "<span class="tex-font-style-tt">eb</span>" because it can be immediately compressed to "<span class="tex-font-style-tt">a</span>".</p>
