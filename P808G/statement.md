## Description

<div><p>Berland has a long and glorious history. To increase awareness about it among younger citizens, King of Berland decided to compose an anthem.</p><p>Though there are lots and lots of victories in history of Berland, there is the one that stand out the most. King wants to mention it in the anthem as many times as possible.</p><p>He has already composed major part of the anthem and now just needs to fill in some letters. King asked you to help him with this work.</p><p>The anthem is the string <span class="tex-span"><i>s</i></span> of no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> small Latin letters and question marks. The most glorious victory is the string <span class="tex-span"><i>t</i></span> of no more than <span class="tex-span">10<sup class="upper-index">5</sup></span> small Latin letters. You should replace all the question marks with small Latin letters in such a way that the number of occurrences of string <span class="tex-span"><i>t</i></span> in string <span class="tex-span"><i>s</i></span> is maximal.</p><p>Note that the occurrences of string <span class="tex-span"><i>t</i></span> in <span class="tex-span"><i>s</i></span> can overlap. Check the third example for clarification.</p></div><div class="input-specification"><p>The first line contains string of small Latin letters and question marks <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains string of small Latin letters <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">5</sup></span>).</p><p><span class="tex-font-style-bf">Product of lengths of strings <span class="tex-span">|<i>s</i>|·|<i>t</i>|</span> won't exceed <span class="tex-span">10<sup class="upper-index">7</sup></span>.</span></p></div><div class="output-specification"><p>Output the maximum number of occurrences of string <span class="tex-span"><i>t</i></span> you can achieve by replacing all the question marks in string <span class="tex-span"><i>s</i></span> with small Latin letters.</p></div>

## Input

<p>The first line contains string of small Latin letters and question marks <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains string of small Latin letters <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ |<i>t</i>| ≤ 10<sup class="upper-index">5</sup></span>).</p><p><span class="tex-font-style-bf">Product of lengths of strings <span class="tex-span">|<i>s</i>|·|<i>t</i>|</span> won't exceed <span class="tex-span">10<sup class="upper-index">7</sup></span>.</span></p>

## Output

<p>Output the maximum number of occurrences of string <span class="tex-span"><i>t</i></span> you can achieve by replacing all the question marks in string <span class="tex-span"><i>s</i></span> with small Latin letters.</p>





```input1
winlose???winl???w??
win

```




```input2
glo?yto?e??an?
or

```




```input3
??c?????
abcab

```




```output1
5

```




```output2
3

```




```output3
2

```



## Note

<p>In the first example the resulting string <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-tt">"winlose<span class="tex-font-style-bf">win</span>winl<span class="tex-font-style-bf">win</span>w<span class="tex-font-style-bf">in</span>"</span></p><p>In the second example the resulting string <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-tt">"glo<span class="tex-font-style-bf">r</span>yto<span class="tex-font-style-bf">r</span>e<span class="tex-font-style-bf">or</span>an<span class="tex-font-style-bf">d</span>"</span>. The last letter of the string can be arbitrary.</p><p>In the third example occurrences of string <span class="tex-span"><i>t</i></span> are overlapping. String <span class="tex-span"><i>s</i></span> with maximal number of occurrences of <span class="tex-span"><i>t</i></span> is <span class="tex-font-style-tt">"<span class="tex-font-style-bf">ab</span>c<span class="tex-font-style-bf">abcab</span>"</span>.</p>
