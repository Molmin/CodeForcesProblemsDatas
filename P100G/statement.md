## Description

<div><p>The famous singer, Aryo, is going to publish a new album of his great work!</p><p>Unfortunately these days, there are many albums, Aryo wants to choose a new name for his album, a name that has not been used or at least has not been used recently.</p><p>He has a list of all used album names together with the year the albums were published. He also has a list of suitable names for his album.</p><p>If he finds a suitable name which has not been used before, he'll use it. Otherwise he will use the name which was used as long ago as possible. If two such names are found (that haven't been used or were used at the same year), he uses the name that is alphabetically latest.</p><p>Help him name his album.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of used names. </p><p>The following <span class="tex-span"><i>n</i></span> lines each contain a string (the album name) and an integer (the year album was published). Album names are made of lowercase Latin letters and contain at most <span class="tex-span">14</span> letters. The year is in range <span class="tex-span">[1900, 2011]</span>.</p><p>The following line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>), the number of suitable album names.</p><p>The following <span class="tex-span"><i>m</i></span> lines each contain a string — a suitable name. It contains at most <span class="tex-span">14</span> lowercase Latin letters.</p><p>All album names and suitable names are <span class="tex-font-style-underline">non-empty</span>.</p></div><div class="output-specification"><p>Write a single string. The name of the new album.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of used names. </p><p>The following <span class="tex-span"><i>n</i></span> lines each contain a string (the album name) and an integer (the year album was published). Album names are made of lowercase Latin letters and contain at most <span class="tex-span">14</span> letters. The year is in range <span class="tex-span">[1900, 2011]</span>.</p><p>The following line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">4</sup></span>), the number of suitable album names.</p><p>The following <span class="tex-span"><i>m</i></span> lines each contain a string — a suitable name. It contains at most <span class="tex-span">14</span> lowercase Latin letters.</p><p>All album names and suitable names are <span class="tex-font-style-underline">non-empty</span>.</p>

## Output

<p>Write a single string. The name of the new album.</p>





```input1
3
eyesonme 2008
anewdayhascome 2002
oneheart 2003
2
oneheart
bienbien

```




```input2
2
nasimevasl 2003
basetareha 2006
2
nasimevasl
basetareha

```




```output1
bienbien

```




```output2
nasimevasl

```


