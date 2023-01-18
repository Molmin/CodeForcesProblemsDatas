## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span> and should process <span class="tex-span"><i>m</i></span> queries. Each query is described by two 1-based indices <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and integer <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span>. It means that you should cyclically shift the substring <span class="tex-span"><i>s</i>[<i>l</i><sub class="lower-index"><i>i</i></sub>... <i>r</i><sub class="lower-index"><i>i</i></sub>]</span> <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> times. The queries should be processed one after another in the order they are given.</p><p>One operation of a cyclic shift (rotation) is equivalent to moving the last character to the position of the first character and shifting all other characters one position to the right.</p><p>For example, if the string <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-tt">abacaba</span> and the query is <span class="tex-span"><i>l</i><sub class="lower-index">1</sub> = 3, <i>r</i><sub class="lower-index">1</sub> = 6, <i>k</i><sub class="lower-index">1</sub> = 1</span> then the answer is <span class="tex-font-style-tt">abbacaa</span>. If after that we would process the query <span class="tex-span"><i>l</i><sub class="lower-index">2</sub> = 1, <i>r</i><sub class="lower-index">2</sub> = 4, <i>k</i><sub class="lower-index">2</sub> = 2</span> then we would get the string <span class="tex-font-style-tt">baabcaa</span>.</p></div><div class="input-specification"><p>The first line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10 000</span>) in its initial state, where <span class="tex-span">|<i>s</i>|</span> stands for the length of <span class="tex-span"><i>s</i></span>. It contains only lowercase English letters.</p><p>Second line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 300</span>)&nbsp;— the number of queries.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|, 1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the description of the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>Print the resulting string <span class="tex-span"><i>s</i></span> after processing all <span class="tex-span"><i>m</i></span> queries.</p></div>

## Input

<p>The first line of the input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10 000</span>) in its initial state, where <span class="tex-span">|<i>s</i>|</span> stands for the length of <span class="tex-span"><i>s</i></span>. It contains only lowercase English letters.</p><p>Second line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 300</span>)&nbsp;— the number of queries.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ |<i>s</i>|, 1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the description of the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>Print the resulting string <span class="tex-span"><i>s</i></span> after processing all <span class="tex-span"><i>m</i></span> queries.</p>





```input1
abacaba
2
3 6 1
1 4 2

```




```output1
baabcaa

```



## Note

<p>The sample is described in problem statement.</p>
