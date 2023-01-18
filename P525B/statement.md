## Description

<div><p>Pasha got a very beautiful string <span class="tex-span"><i>s</i></span> for his birthday, the string consists of lowercase Latin letters. The letters in the string are numbered from 1 to <span class="tex-span">|<i>s</i>|</span> from left to right, where <span class="tex-span">|<i>s</i>|</span> is the length of the given string.</p><p>Pasha didn't like his present very much so he decided to change it. After his birthday Pasha spent <span class="tex-span"><i>m</i></span> days performing the following transformations on his string&nbsp;—&nbsp;each day he chose integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-font-style-bf">reversed</span> a piece of string (a segment) from position <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to position <span class="tex-span">|<i>s</i>| - <i>a</i><sub class="lower-index"><i>i</i></sub> + 1</span>. It is guaranteed that <span class="tex-span">2·<i>a</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|</span>.</p><p>You face the following task: determine what Pasha's string will look like after <span class="tex-span"><i>m</i></span> days.</p></div><div class="input-specification"><p>The first line of the input contains Pasha's string <span class="tex-span"><i>s</i></span> of length from <span class="tex-span">2</span> to <span class="tex-span">2·10<sup class="upper-index">5</sup></span> characters, consisting of lowercase Latin letters.</p><p>The second line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp; the number of days when Pasha changed his string.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space-separated elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span">2·<i>a</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|</span>)&nbsp;—&nbsp;the position from which Pasha started transforming the string on the <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>In the first line of the output print what Pasha's string <span class="tex-span"><i>s</i></span> will look like after <span class="tex-span"><i>m</i></span> days.</p></div>

## Input

<p>The first line of the input contains Pasha's string <span class="tex-span"><i>s</i></span> of length from <span class="tex-span">2</span> to <span class="tex-span">2·10<sup class="upper-index">5</sup></span> characters, consisting of lowercase Latin letters.</p><p>The second line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp; the number of days when Pasha changed his string.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space-separated elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span>; <span class="tex-span">2·<i>a</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|</span>)&nbsp;—&nbsp;the position from which Pasha started transforming the string on the <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>In the first line of the output print what Pasha's string <span class="tex-span"><i>s</i></span> will look like after <span class="tex-span"><i>m</i></span> days.</p>





```input1
abcdef
1
2

```




```input2
vwxyz
2
2 2

```




```input3
abcdef
3
1 2 3

```




```output1
aedcbf

```




```output2
vwxyz

```




```output3
fbdcea

```


