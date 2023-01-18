## Description

<div><p>Daniel has a string <span class="tex-span"><i>s</i></span>, consisting of lowercase English letters and period signs (characters '<span class="tex-font-style-tt">.</span>'). Let's define the operation of <span class="tex-font-style-it">replacement</span> as the following sequence of steps: find a substring "<span class="tex-font-style-tt">..</span>" (two consecutive periods) in string <span class="tex-span"><i>s</i></span>, of all occurrences of the substring let's choose the first one, and replace this substring with string "<span class="tex-font-style-tt">.</span>". In other words, during the replacement operation, the first two consecutive periods are replaced by one. If string <span class="tex-span"><i>s</i></span> contains no two consecutive periods, then nothing happens.</p><p>Let's define <span class="tex-span"><i>f</i>(<i>s</i>)</span> as the minimum number of operations of <span class="tex-font-style-it">replacement</span> to perform, so that the string does not have any two consecutive periods left.</p><p>You need to process <span class="tex-span"><i>m</i></span> queries, the <span class="tex-span"><i>i</i></span>-th results in that the character at position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) of string <span class="tex-span"><i>s</i></span> is assigned value <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. After each operation you have to calculate and output the value of <span class="tex-span"><i>f</i>(<i>s</i>)</span>.</p><p>Help Daniel to process all queries.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300 000</span>) the length of the string and the number of queries.</p><p>The second line contains string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase English letters and period signs.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the descriptions of queries. The <span class="tex-span"><i>i</i></span>-th line contains integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — a lowercas English letter or a period sign), describing the query of assigning symbol <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> to position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> numbers, one per line, the <span class="tex-span"><i>i</i></span>-th of these numbers must be equal to the value of <span class="tex-span"><i>f</i>(<i>s</i>)</span> after performing the <span class="tex-span"><i>i</i></span>-th assignment.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 300 000</span>) the length of the string and the number of queries.</p><p>The second line contains string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase English letters and period signs.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain the descriptions of queries. The <span class="tex-span"><i>i</i></span>-th line contains integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> — a lowercas English letter or a period sign), describing the query of assigning symbol <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> to position <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> numbers, one per line, the <span class="tex-span"><i>i</i></span>-th of these numbers must be equal to the value of <span class="tex-span"><i>f</i>(<i>s</i>)</span> after performing the <span class="tex-span"><i>i</i></span>-th assignment.</p>





```input1
10 3
.b..bz....
1 h
3 c
9 f

```




```input2
4 4
.cc.
2 .
3 .
2 a
1 a

```




```output1
4
3
1

```




```output2
1
3
1
1

```



## Note

<p>Note to the first sample test (replaced periods are enclosed in square brackets).</p><p>The original string is "<span class="tex-font-style-tt">.b..bz....</span>".</p><ul><li> after the first query <span class="tex-span"><i>f</i>(</span><span class="tex-font-style-tt">hb..bz....</span><span class="tex-span">)</span> = 4&nbsp;&nbsp;&nbsp;&nbsp;("<span class="tex-font-style-tt">hb[..]bz....</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hb.bz[..]..</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hb.bz[..].</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hb.bz[..]</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hb.bz.</span>")</li><li> after the second query <span class="tex-span"><i>f</i>(</span><span class="tex-font-style-tt">hbс.bz....</span><span class="tex-span">)</span> = 3&nbsp;&nbsp;&nbsp;&nbsp;("<span class="tex-font-style-tt">hbс.bz[..]..</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hbс.bz[..].</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hbс.bz[..]</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hbс.bz.</span>")</li><li> after the third query <span class="tex-span"><i>f</i>(</span><span class="tex-font-style-tt">hbс.bz..f.</span><span class="tex-span">)</span> = 1&nbsp;&nbsp;&nbsp;&nbsp;("<span class="tex-font-style-tt">hbс.bz[..]f.</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">hbс.bz.f.</span>")</li></ul><p>Note to the second sample test.</p><p>The original string is "<span class="tex-font-style-tt">.cc.</span>".</p><ul><li> after the first query: <span class="tex-span"><i>f</i>(</span><span class="tex-font-style-tt">..c.</span><span class="tex-span">)</span> = 1&nbsp;&nbsp;&nbsp;&nbsp;("<span class="tex-font-style-tt">[..]c.</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">.c.</span>")</li><li> after the second query: <span class="tex-span"><i>f</i>(</span><span class="tex-font-style-tt">....</span><span class="tex-span">)</span> = 3&nbsp;&nbsp;&nbsp;&nbsp;("<span class="tex-font-style-tt">[..]..</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">[..].</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">[..]</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">.</span>")</li><li> after the third query: <span class="tex-span"><i>f</i>(</span><span class="tex-font-style-tt">.a..</span><span class="tex-span">)</span> = 1&nbsp;&nbsp;&nbsp;&nbsp;("<span class="tex-font-style-tt">.a[..]</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">.a.</span>")</li><li> after the fourth query: <span class="tex-span"><i>f</i>(</span><span class="tex-font-style-tt">aa..</span><span class="tex-span">)</span> = 1&nbsp;&nbsp;&nbsp;&nbsp;("<span class="tex-font-style-tt">aa[..]</span>" <span class="tex-span"> → </span> "<span class="tex-font-style-tt">aa.</span>")</li></ul>
