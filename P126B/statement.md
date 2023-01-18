## Description

<div><p>Asterix, Obelix and their temporary buddies Suffix and Prefix has finally found the Harmony temple. However, its doors were firmly locked and even Obelix had no luck opening them.</p><p>A little later they found a string <span class="tex-span"><i>s</i></span>, carved on a rock below the temple's gates. Asterix supposed that that's the password that opens the temple and read the string aloud. However, nothing happened. Then Asterix supposed that a password is some substring <span class="tex-span"><i>t</i></span> of the string <span class="tex-span"><i>s</i></span>.</p><p>Prefix supposed that the substring <span class="tex-span"><i>t</i></span> is the beginning of the string <span class="tex-span"><i>s</i></span>; Suffix supposed that the substring <span class="tex-span"><i>t</i></span> should be the end of the string <span class="tex-span"><i>s</i></span>; and Obelix supposed that <span class="tex-span"><i>t</i></span> should be located somewhere inside the string <span class="tex-span"><i>s</i></span>, that is, <span class="tex-span"><i>t</i></span> is neither its beginning, nor its end.</p><p>Asterix chose the substring <span class="tex-span"><i>t</i></span> so as to please all his companions. Besides, from all acceptable variants Asterix chose the longest one (as Asterix loves long strings). When Asterix read the substring <span class="tex-span"><i>t</i></span> aloud, the temple doors opened. </p><p>You know the string <span class="tex-span"><i>s</i></span>. Find the substring <span class="tex-span"><i>t</i></span> or determine that such substring does not exist and all that's been written above is just a nice legend.</p></div><div class="input-specification"><p>You are given the string <span class="tex-span"><i>s</i></span> whose length can vary from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span> (inclusive), consisting of small Latin letters.</p></div><div class="output-specification"><p>Print the string <span class="tex-span"><i>t</i></span>. If a suitable <span class="tex-span"><i>t</i></span> string does not exist, then print "<span class="tex-font-style-tt">Just a legend</span>" without the quotes.</p></div>

## Input

<p>You are given the string <span class="tex-span"><i>s</i></span> whose length can vary from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span> (inclusive), consisting of small Latin letters.</p>

## Output

<p>Print the string <span class="tex-span"><i>t</i></span>. If a suitable <span class="tex-span"><i>t</i></span> string does not exist, then print "<span class="tex-font-style-tt">Just a legend</span>" without the quotes.</p>





```input1
fixprefixsuffix

```




```input2
abcdabc

```




```output1
fix
```




```output2
Just a legend
```


