## Description

<div><p>"QAQ" is a word to denote an expression of crying. Imagine "Q" as eyes with tears and "A" as a mouth.</p><p>Now Diamond has given Bort a string consisting of only uppercase English letters of length <span class="tex-span"><i>n</i></span>. There is a great number of "QAQ" in the string (Diamond is so cute!).</p><center> <img class="tex-graphics" height="259px" src="file://wZgBZaZu.png" style="max-width: 100.0%;max-height: 100.0%;" width="341px"> <span class="tex-font-size-tiny">illustration by 猫屋 https://twitter.com/nekoyaliu</span> </center><p>Bort wants to know how many subsequences "<span class="tex-font-style-tt">QAQ</span>" are in the string Diamond has given. Note that the letters "<span class="tex-font-style-tt">QAQ</span>" don't have to be consecutive, but the order of letters should be exact.</p></div><div class="input-specification"><p>The only line contains a string of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). It's guaranteed that the string only contains uppercase English letters.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of subsequences "<span class="tex-font-style-tt">QAQ</span>" in the string.</p></div>

## Input

<p>The only line contains a string of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). It's guaranteed that the string only contains uppercase English letters.</p>

## Output

<p>Print a single integer&nbsp;— the number of subsequences "<span class="tex-font-style-tt">QAQ</span>" in the string.</p>





```input1
QAQAQYSYIOIWIN

```




```input2
QAQQQZZYNOIWIN

```




```output1
4

```




```output2
3

```



## Note

<p>In the first example there are <span class="tex-span">4</span> subsequences "<span class="tex-font-style-tt">QAQ</span>": "<span class="tex-font-style-tt"><span class="tex-font-style-bf">QAQ</span>AQYSYIOIWIN</span>", "<span class="tex-font-style-tt"><span class="tex-font-style-bf">QA</span>QA<span class="tex-font-style-bf">Q</span>YSYIOIWIN</span>", "<span class="tex-font-style-tt"><span class="tex-font-style-bf">Q</span>AQ<span class="tex-font-style-bf">AQ</span>YSYIOIWIN</span>", "<span class="tex-font-style-tt">QA<span class="tex-font-style-bf">QAQ</span>YSYIOIWIN</span>".</p>
