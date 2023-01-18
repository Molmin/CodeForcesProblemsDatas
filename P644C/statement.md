## Description

<div><p>There are some websites that are accessible through several different addresses. For example, for a long time Codeforces was accessible with two hostnames <span class="tex-font-style-tt">codeforces.com</span> and <span class="tex-font-style-tt">codeforces.ru</span>.</p><p>You are given a list of page addresses being queried. For simplicity we consider all addresses to have the form <span class="tex-font-style-tt">http://&lt;hostname&gt;[/&lt;path&gt;]</span>, where:</p><ul> <li> <span class="tex-font-style-tt">&lt;hostname&gt;</span>&nbsp;— server name (consists of words and maybe some dots separating them), </li><li> <span class="tex-font-style-tt">/&lt;path&gt;</span>&nbsp;— optional part, where &lt;path&gt; consists of words separated by slashes. </li></ul><p>We consider two <span class="tex-font-style-tt">&lt;hostname&gt;</span> to correspond to one website if for each query to the first <span class="tex-font-style-tt">&lt;hostname&gt;</span> there will be exactly the same query to the second one and vice versa&nbsp;— for each query to the second <span class="tex-font-style-tt">&lt;hostname&gt;</span> there will be the same query to the first one. Take a look at the samples for further clarifications.</p><p>Your goal is to determine the groups of server names that correspond to one website. Ignore groups consisting of the only server name.</p><p>Please note, that according to the above definition queries <span class="tex-font-style-tt">http://&lt;hostname&gt;</span> and <span class="tex-font-style-tt">http://&lt;hostname&gt;/</span> are different.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of page queries. Then follow <span class="tex-span"><i>n</i></span> lines each containing exactly one address. Each address is of the form <span class="tex-font-style-tt">http://&lt;hostname&gt;[/&lt;path&gt;]</span>, where:</p><ul> <li> <span class="tex-font-style-tt">&lt;hostname&gt;</span> consists of lowercase English letters and dots, there are no two consecutive dots, <span class="tex-font-style-tt">&lt;hostname&gt;</span> doesn't start or finish with a dot. The length of <span class="tex-font-style-tt">&lt;hostname&gt;</span> is positive and doesn't exceed <span class="tex-span">20</span>. </li><li> <span class="tex-font-style-tt">&lt;path&gt;</span> consists of lowercase English letters, dots and slashes. There are no two consecutive slashes, <span class="tex-font-style-tt">&lt;path&gt;</span> doesn't start with a slash and its length doesn't exceed <span class="tex-span">20</span>. </li></ul><p>Addresses are not guaranteed to be distinct.</p></div><div class="output-specification"><p>First print <span class="tex-span"><i>k</i></span>&nbsp;— the number of groups of server names that correspond to one website. You should count only groups of size greater than one.</p><p>Next <span class="tex-span"><i>k</i></span> lines should contain the description of groups, one group per line. For each group print all server names separated by a single space. You are allowed to print both groups and names inside any group in arbitrary order.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of page queries. Then follow <span class="tex-span"><i>n</i></span> lines each containing exactly one address. Each address is of the form <span class="tex-font-style-tt">http://&lt;hostname&gt;[/&lt;path&gt;]</span>, where:</p><ul> <li> <span class="tex-font-style-tt">&lt;hostname&gt;</span> consists of lowercase English letters and dots, there are no two consecutive dots, <span class="tex-font-style-tt">&lt;hostname&gt;</span> doesn't start or finish with a dot. The length of <span class="tex-font-style-tt">&lt;hostname&gt;</span> is positive and doesn't exceed <span class="tex-span">20</span>. </li><li> <span class="tex-font-style-tt">&lt;path&gt;</span> consists of lowercase English letters, dots and slashes. There are no two consecutive slashes, <span class="tex-font-style-tt">&lt;path&gt;</span> doesn't start with a slash and its length doesn't exceed <span class="tex-span">20</span>. </li></ul><p>Addresses are not guaranteed to be distinct.</p>

## Output

<p>First print <span class="tex-span"><i>k</i></span>&nbsp;— the number of groups of server names that correspond to one website. You should count only groups of size greater than one.</p><p>Next <span class="tex-span"><i>k</i></span> lines should contain the description of groups, one group per line. For each group print all server names separated by a single space. You are allowed to print both groups and names inside any group in arbitrary order.</p>





```input1
10
http://abacaba.ru/test
http://abacaba.ru/
http://abacaba.com
http://abacaba.com/test
http://abacaba.de/
http://abacaba.ru/test
http://abacaba.de/test
http://abacaba.com/
http://abacaba.com/t
http://abacaba.com/test

```




```input2
14
http://c
http://ccc.bbbb/aba..b
http://cba.com
http://a.c/aba..b/a
http://abc/
http://a.c/
http://ccc.bbbb
http://ab.ac.bc.aa/
http://a.a.a/
http://ccc.bbbb/
http://cba.com/
http://cba.com/aba..b
http://a.a.a/aba..b/a
http://abc/aba..b/a

```




```output1
1
http://abacaba.de http://abacaba.ru 

```




```output2
2
http://cba.com http://ccc.bbbb 
http://a.a.a http://a.c http://abc 

```


