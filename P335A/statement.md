## Description

<div><p>Piegirl is buying stickers for a project. Stickers come on sheets, and each sheet of stickers contains exactly <span class="tex-span"><i>n</i></span> stickers. Each sticker has exactly one character printed on it, so a sheet of stickers can be described by a string of length <span class="tex-span"><i>n</i></span>. Piegirl wants to create a string <span class="tex-span"><i>s</i></span> using stickers. She may buy as many sheets of stickers as she wants, and may specify any string of length <span class="tex-span"><i>n</i></span> for the sheets, but all the sheets must be identical, so the string is the same for all sheets. Once she attains the sheets of stickers, she will take some of the stickers from the sheets and arrange (in any order) them to form <span class="tex-span"><i>s</i></span>. Determine the minimum number of sheets she has to buy, and provide a string describing a possible sheet of stickers she should buy.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>), consisting of lowercase English characters only. The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>On the first line, print the minimum number of sheets Piegirl has to buy. On the second line, print a string consisting of <span class="tex-span"><i>n</i></span> lower case English characters. This string should describe a sheet of stickers that Piegirl can buy in order to minimize the number of sheets. If Piegirl cannot possibly form the string <span class="tex-span"><i>s</i></span>, print instead a single line with the number -1.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>), consisting of lowercase English characters only. The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>).</p>

## Output

<p>On the first line, print the minimum number of sheets Piegirl has to buy. On the second line, print a string consisting of <span class="tex-span"><i>n</i></span> lower case English characters. This string should describe a sheet of stickers that Piegirl can buy in order to minimize the number of sheets. If Piegirl cannot possibly form the string <span class="tex-span"><i>s</i></span>, print instead a single line with the number -1.</p>





```input1
banana
4

```




```input2
banana
3

```




```input3
banana
2

```




```output1
2
baan

```




```output2
3
nab

```




```output3
-1

```



## Note

<p>In the second example, Piegirl can order 3 sheets of stickers with the characters "<span class="tex-font-style-tt">nab</span>". She can take characters "<span class="tex-font-style-tt">nab</span>" from the first sheet, "<span class="tex-font-style-tt">na</span>" from the second, and "<span class="tex-font-style-tt">a</span>" from the third, and arrange them to from "<span class="tex-font-style-tt">banana</span>".</p>
