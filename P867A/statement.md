## Description

<div><p>As you may know, MemSQL has American offices in both San Francisco and Seattle. Being a manager in the company, you travel a lot between the two cities, always by plane.</p><p>You prefer flying from Seattle to San Francisco than in the other direction, because it's warmer in San Francisco. You are so busy that you don't remember the number of flights you have made in either direction. However, for each of the last <span class="tex-span"><i>n</i></span> days you know whether you were in San Francisco office or in Seattle office. You always fly at nights, so you never were at both offices on the same day. Given this information, determine if you flew more times from Seattle to San Francisco during the last <span class="tex-span"><i>n</i></span> days, or not.</p></div><div class="input-specification"><p>The first line of input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of days.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span> consisting of only capital '<span class="tex-font-style-tt">S</span>' and '<span class="tex-font-style-tt">F</span>' letters. If the <span class="tex-span"><i>i</i></span>-th letter is '<span class="tex-font-style-tt">S</span>', then you were in Seattle office on that day. Otherwise you were in San Francisco. The days are given in chronological order, i.e. today is the last day in this sequence.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if you flew more times from Seattle to San Francisco, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of days.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span> consisting of only capital '<span class="tex-font-style-tt">S</span>' and '<span class="tex-font-style-tt">F</span>' letters. If the <span class="tex-span"><i>i</i></span>-th letter is '<span class="tex-font-style-tt">S</span>', then you were in Seattle office on that day. Otherwise you were in San Francisco. The days are given in chronological order, i.e. today is the last day in this sequence.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if you flew more times from Seattle to San Francisco, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
4
FSSF

```




```input2
2
SF

```




```input3
10
FFFFFFFFFF

```




```input4
10
SSFFSFFSFF

```




```output1
NO

```




```output2
YES

```




```output3
NO

```




```output4
YES

```



## Note

<p>In the first example you were initially at San Francisco, then flew to Seattle, were there for two days and returned to San Francisco. You made one flight in each direction, so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the second example you just flew from Seattle to San Francisco, so the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the third example you stayed the whole period in San Francisco, so the answer is "<span class="tex-font-style-tt">NO</span>".</p><p>In the fourth example if you replace '<span class="tex-font-style-tt">S</span>' with ones, and '<span class="tex-font-style-tt">F</span>' with zeros, you'll get the first few digits of <span class="tex-span">π</span> in binary representation. Not very useful information though.</p>
