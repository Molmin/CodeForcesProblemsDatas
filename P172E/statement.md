## Description

<div><p><span class="tex-font-style-it">This problem is about imaginary languages BHTML and BCSS, which slightly resemble HTML and CSS. Read the problem statement carefully as the resemblance is rather slight and the problem uses very simplified analogs.</span></p><p>You are given a BHTML document that resembles HTML but is much simpler. It is recorded as a sequence of opening and closing tags. A tag that looks like "<span class="tex-font-style-tt">&lt;tagname&gt;</span>" is called an opening tag and a tag that looks like "<span class="tex-font-style-tt">&lt;/tagname&gt;</span>" is called a closing tag. Besides, there are self-closing tags that are written as "<span class="tex-font-style-tt">&lt;tagname/&gt;</span>" and in this problem they are fully equivalent to "<span class="tex-font-style-tt">&lt;tagname&gt;&lt;/tagname&gt;</span>". All tagnames in this problem are strings consisting of lowercase Latin letters with length from 1 to 10 characters. Tagnames of different tags may coincide.</p><p>The document tags form a correct bracket sequence, that is, we can obtain an empty sequence from the given one using the following operations: </p><ul> <li> remove any self-closing tag "<span class="tex-font-style-tt">&lt;tagname/&gt;</span>", </li><li> remove a pair of an opening and a closing tag that go consecutively (in this order) and have the same names. In other words, remove substring "<span class="tex-font-style-tt">&lt;tagname&gt;&lt;/tagname&gt;</span>". </li></ul><p>For example, you may be given such document: "<span class="tex-font-style-tt">&lt;header&gt;&lt;p&gt;&lt;a/&gt;&lt;b&gt;&lt;/b&gt;&lt;/p&gt;&lt;/header&gt;&lt;footer&gt;&lt;/footer&gt;</span>" but you may not be given documents "<span class="tex-font-style-tt">&lt;a&gt;</span>", "<span class="tex-font-style-tt">&lt;a&gt;&lt;/b&gt;</span>", "<span class="tex-font-style-tt">&lt;/a&gt;&lt;a&gt;</span>" or "<span class="tex-font-style-tt">&lt;a&gt;&lt;b&gt;&lt;/a&gt;&lt;/b&gt;</span>".</p><p>Obviously, for any opening tag there is the only matching closing one — each such pair is called an <span class="tex-font-style-it">element</span>. A self-closing tag also is an element. Let's consider that one element is nested inside another one, if tags of the first element are between tags of the second one. An element is not nested to itself. For instance, in the example above element "<span class="tex-font-style-tt">b</span>" is nested in "<span class="tex-font-style-tt">header</span>" and in "<span class="tex-font-style-tt">p</span>", but it isn't nested in "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">footer</span>", also it isn't nested to itself ("<span class="tex-font-style-tt">b</span>"). Element "<span class="tex-font-style-tt">header</span>" has three elements nested in it, and "<span class="tex-font-style-tt">footer</span>" has zero.</p><p>We need the BCSS rules to apply styles when displaying elements of the BHTML documents. Each rule is recorded as a subsequence of words "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> ... <span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span></span>". This rule has effect over all such elements <span class="tex-span"><i>t</i></span>, which satisfy both conditions from the list:</p><ul> <li> there is a sequence of nested elements with tagnames "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span></span>", "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span></span>", ..., "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span></span>" (that is, the second element is nested in the first one, the third element is nested in the second one and so on), </li><li> this sequence ends with element <span class="tex-span"><i>t</i></span> (i.e. tagname of element <span class="tex-span"><i>t</i></span> equals "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i><sub class="lower-index"><i>n</i></sub></span></span>"). </li></ul><p>For example, element "<span class="tex-font-style-tt">b</span>" meets the conditions of the rule "<span class="tex-font-style-tt">a b</span>" if for element "<span class="tex-font-style-tt">b</span>" exists element "<span class="tex-font-style-tt">a</span>" in which it is nested. Element "<span class="tex-font-style-tt">c</span>" meets the conditions of the rule "<span class="tex-font-style-tt">a b b c</span>", if three elements exist: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">b</span>", and in the chain "<span class="tex-font-style-tt">a</span>"-"<span class="tex-font-style-tt">b</span>"-"<span class="tex-font-style-tt">b</span>"-"<span class="tex-font-style-tt">c</span>" each following element is nested in the previous one.</p><p>Given a BHTML document and a set of BCSS rules, write a program that determines the number of elements that meet the conditions of each rule.</p></div><div class="input-specification"><p>The first line of the input contains a BHTML-document. The document has length from <span class="tex-span">4</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. The document has a correct structure, doesn't contain spaces or any other unnecessary characters. Tagnames consist of lowercase Latin letters, their lengths are from 1 to 10 characters.</p><p>The second line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200</span>) — the number of queries. Then <span class="tex-span"><i>m</i></span> lines contain the queries, one per line. Each query is a sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the query, and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) is the number of elements in the query. The elements are separated by single spaces. Each query doesn't begin with and doesn't end with a space. Each query element is a sequence of lowercase Latin letters with length from 1 to 10.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>j</i></span>-th line should contain the number of elements of the document that correspond to the <span class="tex-span"><i>j</i></span>-th BCSS-rule. If there are no such elements at all, print on the line <span class="tex-font-style-tt">0</span>.</p></div>

## Input

<p>The first line of the input contains a BHTML-document. The document has length from <span class="tex-span">4</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span> characters. The document has a correct structure, doesn't contain spaces or any other unnecessary characters. Tagnames consist of lowercase Latin letters, their lengths are from 1 to 10 characters.</p><p>The second line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200</span>) — the number of queries. Then <span class="tex-span"><i>m</i></span> lines contain the queries, one per line. Each query is a sequence <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th element of the query, and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) is the number of elements in the query. The elements are separated by single spaces. Each query doesn't begin with and doesn't end with a space. Each query element is a sequence of lowercase Latin letters with length from 1 to 10.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, the <span class="tex-span"><i>j</i></span>-th line should contain the number of elements of the document that correspond to the <span class="tex-span"><i>j</i></span>-th BCSS-rule. If there are no such elements at all, print on the line <span class="tex-font-style-tt">0</span>.</p>





```input1
&lt;a&gt;&lt;b&gt;&lt;b&gt;&lt;/b&gt;&lt;/b&gt;&lt;/a&gt;&lt;a&gt;&lt;b&gt;&lt;/b&gt;&lt;b&gt;&lt;v/&gt;&lt;/b&gt;&lt;/a&gt;&lt;b&gt;&lt;/b&gt;
4
a
a b b
a b
b a

```




```input2
&lt;b&gt;&lt;aa/&gt;&lt;/b&gt;&lt;aa&gt;&lt;b/&gt;&lt;b/&gt;&lt;/aa&gt;
5
aa b
b
aa
b aa
a

```




```output1
2
1
4
0

```




```output2
2
3
2
1
0

```


