## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">What are you doing at the end of the world? Are you busy? Will you save us?</span></div></div><center><p><img class="tex-graphics" src="file://KlUNnWkP.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center><p>Nephren is playing a game with little leprechauns.</p><p>She gives them an infinite array of strings, <span class="tex-span"><i>f</i><sub class="lower-index">0... ∞</sub></span>.</p><p><span class="tex-span"><i>f</i><sub class="lower-index">0</sub></span> is "<span class="tex-font-style-tt">What are you doing at the end of the world? Are you busy? Will you save us?</span>".</p><p>She wants to let more people know about it, so she defines <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub> = </span> "<span class="tex-font-style-tt">What are you doing while sending "</span><span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i> - 1</sub></span><span class="tex-font-style-tt">"? Are you busy? Will you send "</span><span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i> - 1</sub></span><span class="tex-font-style-tt">"?</span>" for all <span class="tex-span"><i>i</i> ≥ 1</span>.</p><p>For example, <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span> is</p><p>"<span class="tex-font-style-tt">What are you doing while sending "What are you doing at the end of the world? Are you busy? Will you save us?"? Are you busy? Will you send "What are you doing at the end of the world? Are you busy? Will you save us?"?</span>". Note that the quotes in the very beginning and in the very end are for clarity and are not a part of <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span>.</p><p>It can be seen that the characters in <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> are letters, question marks, (possibly) quotation marks and spaces.</p><p>Nephren will ask the little leprechauns <span class="tex-span"><i>q</i></span> times. Each time she will let them find the <span class="tex-span"><i>k</i></span>-th character of <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i></sub></span>. The characters are indexed starting from <span class="tex-span">1</span>. If <span class="tex-span"><i>f</i><sub class="lower-index"><i>n</i></sub></span> consists of less than <span class="tex-span"><i>k</i></span> characters, output '<span class="tex-font-style-tt">.</span>' (without quotes).</p><p>Can you answer her queries?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10</span>)&nbsp;— the number of Nephren's questions.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines describes Nephren's question and contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>).</p></div><div class="output-specification"><p>One line containing <span class="tex-span"><i>q</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character in it should be the answer for the <span class="tex-span"><i>i</i></span>-th query.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10</span>)&nbsp;— the number of Nephren's questions.</p><p>Each of the next <span class="tex-span"><i>q</i></span> lines describes Nephren's question and contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>).</p>

## Output

<p>One line containing <span class="tex-span"><i>q</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character in it should be the answer for the <span class="tex-span"><i>i</i></span>-th query.</p>





```input1
3
1 1
1 2
1 111111111111

```




```input2
5
0 69
1 194
1 139
0 47
1 66

```




```input3
10
4 1825
3 75
3 530
4 1829
4 1651
3 187
4 584
4 255
4 774
2 474

```




```output1
Wh.
```




```output2
abdef
```




```output3
Areyoubusy
```



## Note

<p>For the first two examples, refer to <span class="tex-span"><i>f</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span> given in the legend.</p>
