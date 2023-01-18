## Description

<div><p>The main city magazine offers its readers an opportunity to publish their ads. The format of the ad should be like this:</p><p>There are space-separated non-empty words of lowercase and uppercase Latin letters.</p><p>There are hyphen characters <span class="tex-font-style-tt">'-'</span> in some words, their positions set word wrapping points. Word can include more than one hyphen. </p><p>It is guaranteed that there are no adjacent spaces and no adjacent hyphens. No hyphen is adjacent to space. There are no spaces and no hyphens before the first word and after the last word. </p><p>When the word is wrapped, the part of the word before hyphen and the hyphen itself stay on current line and the next part of the word is put on the next line. You can also put line break between two words, in that case the space stays on current line. Check notes for better understanding.</p><p>The ad can occupy no more that <span class="tex-span"><i>k</i></span> lines and should have minimal width. The width of the ad is the maximal length of string (letters, spaces and hyphens are counted) in it.</p><p>You should write a program that will find minimal width of the ad.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains the text of the ad — non-empty space-separated words of lowercase and uppercase Latin letters and hyphens. Total length of the ad don't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p></div><div class="output-specification"><p>Output minimal width of the ad.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains the text of the ad — non-empty space-separated words of lowercase and uppercase Latin letters and hyphens. Total length of the ad don't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> characters.</p>

## Output

<p>Output minimal width of the ad.</p>





```input1
4
garage for sa-le

```




```input2
4
Edu-ca-tion-al Ro-unds are so fun

```




```output1
7

```




```output2
10

```



## Note

<p>Here all spaces are replaced with dots.</p><p>In the first example one of possible results after all word wraps looks like this:</p><pre class="verbatim"><br>garage.<br>for.<br>sa-<br>le<br></pre><p>The second example:</p><pre class="verbatim"><br>Edu-ca-<br>tion-al.<br>Ro-unds.<br>are.so.fun<br></pre>
