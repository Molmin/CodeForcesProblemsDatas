## Description

<div><p>You are given string <span class="tex-span"><i>s</i></span>. Let's call <span class="tex-font-style-tt">word</span> any largest sequence of consecutive symbols without symbols '<span class="tex-font-style-tt">,</span>' (comma) and '<span class="tex-font-style-tt">;</span>' (semicolon). For example, there are four <span class="tex-font-style-tt">words</span> in string "<span class="tex-font-style-tt">aba,123;1a;0</span>": "<span class="tex-font-style-tt">aba</span>", "<span class="tex-font-style-tt">123</span>", "<span class="tex-font-style-tt">1a</span>", "<span class="tex-font-style-tt">0</span>". A word can be empty: for example, the string <span class="tex-span"><i>s</i></span>="<span class="tex-font-style-tt">;;</span>" contains three empty words separated by '<span class="tex-font-style-tt">;</span>'.</p><p>You should find all <span class="tex-font-style-tt">words</span> in the given string that are nonnegative INTEGER numbers without leading zeroes and build by them new string <span class="tex-span"><i>a</i></span>. String <span class="tex-span"><i>a</i></span> should contain all <span class="tex-font-style-tt">words</span> that are numbers separating them by '<span class="tex-font-style-tt">,</span>' (the order of numbers should remain the same as in the string <span class="tex-span"><i>s</i></span>). By all other <span class="tex-font-style-tt">words</span> you should build string <span class="tex-span"><i>b</i></span> in the same way (the order of numbers should remain the same as in the string <span class="tex-span"><i>s</i></span>).</p><p>Here strings "<span class="tex-font-style-tt">101</span>", "<span class="tex-font-style-tt">0</span>" are INTEGER numbers, but "<span class="tex-font-style-tt">01</span>" and "<span class="tex-font-style-tt">1.0</span>" are not.</p><p>For example, for the string <span class="tex-font-style-tt">aba,123;1a;0</span> the string <span class="tex-span"><i>a</i></span> would be equal to "<span class="tex-font-style-tt">123,0</span>" and string <span class="tex-span"><i>b</i></span> would be equal to "<span class="tex-font-style-tt">aba,1a</span>".</p></div><div class="input-specification"><p>The only line of input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>). The string contains only symbols '<span class="tex-font-style-tt">.</span>' (ASCII 46), '<span class="tex-font-style-tt">,</span>' (ASCII 44), '<span class="tex-font-style-tt">;</span>' (ASCII 59), digits, lowercase and uppercase latin letters.</p></div><div class="output-specification"><p>Print the string <span class="tex-span"><i>a</i></span> to the first line and string <span class="tex-span"><i>b</i></span> to the second line. Each string should be surrounded by quotes (ASCII 34).</p><p>If there are no <span class="tex-font-style-tt">words</span> that are numbers print dash (ASCII 45) on the first line. If all <span class="tex-font-style-tt">words</span> are numbers print dash on the second line.</p></div>

## Input

<p>The only line of input contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>). The string contains only symbols '<span class="tex-font-style-tt">.</span>' (ASCII 46), '<span class="tex-font-style-tt">,</span>' (ASCII 44), '<span class="tex-font-style-tt">;</span>' (ASCII 59), digits, lowercase and uppercase latin letters.</p>

## Output

<p>Print the string <span class="tex-span"><i>a</i></span> to the first line and string <span class="tex-span"><i>b</i></span> to the second line. Each string should be surrounded by quotes (ASCII 34).</p><p>If there are no <span class="tex-font-style-tt">words</span> that are numbers print dash (ASCII 45) on the first line. If all <span class="tex-font-style-tt">words</span> are numbers print dash on the second line.</p>





```input1
aba,123;1a;0

```




```input2
1;;01,a0,

```




```input3
1

```




```input4
a

```




```output1
"123,0"
"aba,1a"

```




```output2
"1"
",01,a0,"

```




```output3
"1"
-

```




```output4
-
"a"

```



## Note

<p>In the second example the string <span class="tex-span"><i>s</i></span> contains five words: "<span class="tex-font-style-tt">1</span>", "", "<span class="tex-font-style-tt">01</span>", "<span class="tex-font-style-tt">a0</span>", "".</p>
