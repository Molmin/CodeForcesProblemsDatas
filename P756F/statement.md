## Description

<div><p>Consider the following grammar:</p><ul><li> <span class="tex-font-style-tt">&lt;expression&gt; ::= &lt;term&gt; | &lt;expression&gt; '+' &lt;term&gt;</span></li><li> <span class="tex-font-style-tt">&lt;term&gt; ::= &lt;number&gt; | &lt;number&gt; '-' &lt;number&gt; | &lt;number&gt; '(' &lt;expression&gt; ')'</span></li><li> <span class="tex-font-style-tt">&lt;number&gt; ::= &lt;pos_digit&gt; | &lt;number&gt; &lt;digit&gt;</span></li><li> <span class="tex-font-style-tt">&lt;digit&gt; ::= '0' | &lt;pos_digit&gt;</span></li><li> <span class="tex-font-style-tt">&lt;pos_digit&gt; ::= '1' | '2' | '3' | '4' | '5' | '6' | '7' | '8' | '9'</span></li></ul><p>This grammar describes a number in decimal system using the following rules:</p><ul><li> <span class="tex-font-style-tt">&lt;number&gt;</span> describes itself,</li><li> <span class="tex-font-style-tt">&lt;number&gt;-&lt;number&gt;</span> (<span class="tex-font-style-tt">l-r</span>, <span class="tex-span"><i>l</i> ≤ <i>r</i></span>) describes integer which is concatenation of all integers from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>, written without leading zeros. For example, <span class="tex-font-style-tt">8-11</span> describes <span class="tex-font-style-tt">891011</span>,</li><li> <span class="tex-font-style-tt">&lt;number&gt;(&lt;expression&gt;)</span> describes integer which is concatenation of &lt;number&gt; copies of integer described by <span class="tex-font-style-tt">&lt;expression&gt;</span>,</li><li> <span class="tex-font-style-tt">&lt;expression&gt;+&lt;term&gt;</span> describes integer which is concatenation of integers described by <span class="tex-font-style-tt">&lt;expression&gt;</span> and <span class="tex-font-style-tt">&lt;term&gt;</span>.</li></ul><p>For example, <span class="tex-font-style-tt">2(2-4+1)+2(2(17))</span> describes the integer <span class="tex-font-style-tt">2341234117171717</span>.</p><p>You are given an expression in the given grammar. Print the integer described by it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The only line contains a non-empty string at most <span class="tex-span">10<sup class="upper-index">5</sup></span> characters long which is valid according to the given grammar. In particular, it means that in terms <span class="tex-font-style-tt">l-r</span> <span class="tex-span"><i>l</i> ≤ <i>r</i></span> holds.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the number described by the expression modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line contains a non-empty string at most <span class="tex-span">10<sup class="upper-index">5</sup></span> characters long which is valid according to the given grammar. In particular, it means that in terms <span class="tex-font-style-tt">l-r</span> <span class="tex-span"><i>l</i> ≤ <i>r</i></span> holds.</p>

## Output

<p>Print single integer&nbsp;— the number described by the expression modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
8-11

```




```input2
2(2-4+1)+2(2(17))

```




```input3
1234-5678

```




```input4
1+2+3+4-5+6+7-9

```




```output1
891011

```




```output2
100783079

```




```output3
745428774

```




```output4
123456789

```


