## Description

<div><p>Mike has <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span> each consisting of lowercase English letters. In one move he can choose a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>, erase the first character and append it to the end of the string. For example, if he has the string "<span class="tex-font-style-tt">coolmike</span>", in one move he can transform it into the string "<span class="tex-font-style-tt">oolmikec</span>".</p><p>Now Mike asks himself: what is minimal number of moves that he needs to do in order to make all the strings equal?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of strings.</p><p>This is followed by <span class="tex-span"><i>n</i></span> lines which contain a string each. The <span class="tex-span"><i>i</i></span>-th line corresponding to string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. Lengths of strings are equal. Lengths of each string is positive and don't exceed <span class="tex-span">50</span>.</p></div><div class="output-specification"><p>Print the minimal number of moves Mike needs in order to make all the strings equal or print <span class="tex-span"> - 1</span> if there is no solution.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) — the number of strings.</p><p>This is followed by <span class="tex-span"><i>n</i></span> lines which contain a string each. The <span class="tex-span"><i>i</i></span>-th line corresponding to string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. Lengths of strings are equal. Lengths of each string is positive and don't exceed <span class="tex-span">50</span>.</p>

## Output

<p>Print the minimal number of moves Mike needs in order to make all the strings equal or print <span class="tex-span"> - 1</span> if there is no solution.</p>





```input1
4
xzzwo
zwoxz
zzwox
xzzwo

```




```input2
2
molzv
lzvmo

```




```input3
3
kc
kc
kc

```




```input4
3
aa
aa
ab

```




```output1
5

```




```output2
2

```




```output3
0

```




```output4
-1

```



## Note

<p>In the first sample testcase the optimal scenario is to perform operations in such a way as to transform all strings into "<span class="tex-font-style-tt">zwoxz</span>".</p>
