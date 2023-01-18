## Description

<div><p>Let's define a string <span class="tex-font-style-tt">&lt;x&gt;</span> as an opening tag, where <span class="tex-span"><i>x</i></span> is any small letter of the Latin alphabet. Each opening tag matches a closing tag of the type <span class="tex-font-style-tt">&lt;/x&gt;</span>, where <span class="tex-span"><i>x</i></span> is the same letter.</p><p>Tegs can be nested into each other: in this case one opening and closing tag pair is located inside another pair.</p><p>Let's define the notion of a <span class="tex-font-style-it">XML-text</span>: </p><ul> <li> an empty string is a <span class="tex-font-style-it">XML-text</span> </li><li> if <span class="tex-span"><i>s</i></span> is a <span class="tex-font-style-it">XML-text</span>, then <span class="tex-span"><i>s</i>'</span><span class="tex-font-style-tt">=&lt;a&gt;+</span><span class="tex-span"><i>s</i></span><span class="tex-font-style-tt">+&lt;/a&gt;</span> also is a <span class="tex-font-style-it">XML-text</span>, where <span class="tex-span"><i>a</i></span> is any small Latin letter </li><li> if <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> are <span class="tex-font-style-it">XML-texts</span>, then <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>+<span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> also is a <span class="tex-font-style-it">XML-text</span> </li></ul><p>You are given a XML-text (it is guaranteed that the text is valid), your task is to print in the following form: </p><ul> <li> each tag (opening and closing) is located on a single line </li><li> print before the tag <span class="tex-span">2 * <i>h</i></span> spaces, where <span class="tex-span"><i>h</i></span> is the level of the tag's nestedness. </li></ul></div><div class="input-specification"><p>The input data consists on the only non-empty string — the XML-text, its length does not exceed 1000 characters. It is guaranteed that the text is valid. The text contains no spaces.</p></div><div class="output-specification"><p>Print the given XML-text according to the above-given rules.</p></div>

## Input

<p>The input data consists on the only non-empty string — the XML-text, its length does not exceed 1000 characters. It is guaranteed that the text is valid. The text contains no spaces.</p>

## Output

<p>Print the given XML-text according to the above-given rules.</p>





```input1
&lt;a&gt;&lt;b&gt;&lt;c&gt;&lt;/c&gt;&lt;/b&gt;&lt;/a&gt;

```




```input2
&lt;a&gt;&lt;b&gt;&lt;/b&gt;&lt;d&gt;&lt;c&gt;&lt;/c&gt;&lt;/d&gt;&lt;/a&gt;

```




```output1
&lt;a&gt;
  &lt;b&gt;
    &lt;c&gt;
    &lt;/c&gt;
  &lt;/b&gt;
&lt;/a&gt;

```




```output2
&lt;a&gt;
  &lt;b&gt;
  &lt;/b&gt;
  &lt;d&gt;
    &lt;c&gt;
    &lt;/c&gt;
  &lt;/d&gt;
&lt;/a&gt;

```


