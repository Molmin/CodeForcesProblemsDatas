## Description

<div><p>Harry Potter is on a mission to destroy You-Know-Who's Horcruxes. The first Horcrux that he encountered in the Chamber of Secrets is Tom Riddle's diary. The diary was with Ginny and it forced her to open the Chamber of Secrets. Harry wants to know the different people who had ever possessed the diary to make sure they are not under its influence.</p><p>He has names of <span class="tex-span"><i>n</i></span> people who possessed the diary in order. You need to tell, for each person, if he/she possessed the diary at some point before or not.</p><p>Formally, for a name <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> in the <span class="tex-span"><i>i</i></span>-th line, output "<span class="tex-font-style-tt">YES</span>" (without quotes) if there exists an index <span class="tex-span"><i>j</i></span> such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>j</i> &lt; <i>i</i></span>, otherwise, output "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div><div class="input-specification"><p>First line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of names in the list.</p><p>Next <span class="tex-span"><i>n</i></span> lines each contain a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, consisting of lowercase English letters. The length of each string is between <span class="tex-span">1</span> and <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> lines each containing either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" (without quotes), depending on whether this string was already present in the stream or not.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>First line of input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of names in the list.</p><p>Next <span class="tex-span"><i>n</i></span> lines each contain a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, consisting of lowercase English letters. The length of each string is between <span class="tex-span">1</span> and <span class="tex-span">100</span>.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> lines each containing either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" (without quotes), depending on whether this string was already present in the stream or not.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
6
tom
lucius
ginny
harry
ginny
harry

```




```input2
3
a
a
a

```




```output1
NO
NO
NO
NO
YES
YES

```




```output2
NO
YES
YES

```



## Note

<p>In test case <span class="tex-span">1</span>, for <span class="tex-span"><i>i</i> = 5</span> there exists <span class="tex-span"><i>j</i> = 3</span> such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>j</i> &lt; <i>i</i></span>, which means that answer for <span class="tex-span"><i>i</i> = 5</span> is "<span class="tex-font-style-tt">YES</span>".</p>
