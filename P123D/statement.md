## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span>. Each pair of numbers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> that fulfill the condition <span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|</span>, correspond to a substring of the string <span class="tex-span"><i>s</i></span>, starting in the position <span class="tex-span"><i>l</i></span> and ending in the position <span class="tex-span"><i>r</i></span> (inclusive).</p><p>Let's define the function of two strings <span class="tex-span"><i>F</i>(<i>x</i>, <i>y</i>)</span> like this. We'll find a list of such pairs of numbers for which the corresponding substrings of string <span class="tex-span"><i>x</i></span> are equal to string <span class="tex-span"><i>y</i></span>. Let's sort this list of pairs according to the pair's first number's increasing. The value of function <span class="tex-span"><i>F</i>(<i>x</i>, <i>y</i>)</span> equals the number of non-empty continuous sequences in the list.</p><p>For example: <span class="tex-span"><i>F</i>(<i>babbabbababbab</i>, <i>babb</i>) = 6</span>. The list of pairs is as follows:</p><p><span class="tex-span">(1, 4), (4, 7), (9, 12)</span></p><p>Its continuous sequences are: </p><ul> <li> <span class="tex-span">(1, 4)</span> </li><li> <span class="tex-span">(4, 7)</span> </li><li> <span class="tex-span">(9, 12)</span> </li><li> <span class="tex-span">(1, 4), (4, 7)</span> </li><li> <span class="tex-span">(4, 7), (9, 12)</span> </li><li> <span class="tex-span">(1, 4), (4, 7), (9, 12)</span> </li></ul><p>Your task is to calculate for the given string <span class="tex-span"><i>s</i></span> the sum <span class="tex-span"><i>F</i>(<i>s</i>, <i>x</i>)</span> for all <span class="tex-span"><i>x</i></span>, that <span class="tex-span"><i>x</i></span> belongs to the set of all substrings of a string <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The only line contains the given string <span class="tex-span"><i>s</i></span>, consisting only of small Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print the single number — the sought sum.</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p></div>

## Input

<p>The only line contains the given string <span class="tex-span"><i>s</i></span>, consisting only of small Latin letters (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print the single number — the sought sum.</p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p>





```input1
aaaa

```




```input2
abcdef

```




```input3
abacabadabacaba

```




```output1
20

```




```output2
21

```




```output3
188

```



## Note

<p>In the first sample the function values at <span class="tex-span"><i>x</i></span> equal to "a", "aa", "aaa" and "aaaa" equal 10, 6, 3 and 1 correspondingly.</p><p>In the second sample for any satisfying <span class="tex-span"><i>x</i></span> the function value is 1.</p>
