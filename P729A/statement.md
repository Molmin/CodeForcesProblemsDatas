## Description

<div><p>Polycarp has interviewed Oleg and has written the interview down without punctuation marks and spaces to save time. Thus, the interview is now a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters.</p><p>There is a filler word <span class="tex-font-style-tt">ogo</span> in Oleg's speech. All words that can be obtained from <span class="tex-font-style-tt">ogo</span> by adding <span class="tex-font-style-tt">go</span> several times to the end of it are also considered to be fillers. For example, the words <span class="tex-font-style-tt">ogo</span>, <span class="tex-font-style-tt">ogogo</span>, <span class="tex-font-style-tt">ogogogo</span> are fillers, but the words <span class="tex-font-style-tt">go</span>, <span class="tex-font-style-tt">og</span>, <span class="tex-font-style-tt">ogog</span>, <span class="tex-font-style-tt">ogogog</span> and <span class="tex-font-style-tt">oggo</span> are not fillers.</p><p>The fillers have maximal size, for example, for <span class="tex-font-style-tt">ogogoo</span> speech we can't consider <span class="tex-font-style-tt">ogo</span> a filler and <span class="tex-font-style-tt">goo</span> as a normal phrase. We should consider <span class="tex-font-style-tt">ogogo</span> as a filler here.</p><p>To print the interview, Polycarp has to replace each of the fillers with three asterisks. Note that a filler word is replaced with exactly three asterisks regardless of its length.</p><p>Polycarp has dealt with this problem in no time. Can you do the same? The clock is ticking!</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the interview.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p></div><div class="output-specification"><p>Print the interview text after the replacement of each of the fillers with "<span class="tex-font-style-tt">***</span>". It is allowed for the substring "<span class="tex-font-style-tt">***</span>" to have several consecutive occurences.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the interview.</p><p>The second line contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters.</p>

## Output

<p>Print the interview text after the replacement of each of the fillers with "<span class="tex-font-style-tt">***</span>". It is allowed for the substring "<span class="tex-font-style-tt">***</span>" to have several consecutive occurences.</p>





```input1
7
aogogob

```




```input2
13
ogogmgogogogo

```




```input3
9
ogoogoogo

```




```output1
a***b

```




```output2
***gmg***

```




```output3
*********

```



## Note

<p>The first sample contains one filler word <span class="tex-font-style-tt">ogogo</span>, so the interview for printing is "<span class="tex-font-style-tt">a***b</span>".</p><p>The second sample contains two fillers <span class="tex-font-style-tt">ogo</span> and <span class="tex-font-style-tt">ogogogo</span>. Thus, the interview is transformed to "<span class="tex-font-style-tt">***gmg***</span>".</p>
