## Description

<div><p>Once little Vasya read an article in a magazine on how to make beautiful handmade garland from colored paper. Vasya immediately went to the store and bought <span class="tex-span"><i>n</i></span> colored sheets of paper, the area of each sheet is 1 square meter.</p><p>The garland must consist of exactly <span class="tex-span"><i>m</i></span> pieces of colored paper of arbitrary area, each piece should be of a certain color. To make the garland, Vasya can arbitrarily cut his existing colored sheets into pieces. Vasya is not obliged to use all the sheets to make the garland.</p><p>Vasya wants the garland to be as attractive as possible, so he wants to maximize the total area of ​​<span class="tex-span"><i>m</i></span> pieces of paper in the garland. Calculate what the maximum total area of ​​the pieces of paper in the garland Vasya can get.</p></div><div class="input-specification"><p>The first line contains a non-empty sequence of <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) small English letters ("<span class="tex-font-style-tt">a</span>"<span class="tex-span">...</span>"<span class="tex-font-style-tt">z</span>"). Each letter means that Vasya has a sheet of paper of the corresponding color.</p><p>The second line contains a non-empty sequence of <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) small English letters that correspond to the colors of the pieces of paper in the garland that Vasya wants to make.</p></div><div class="output-specification"><p>Print an integer that is the maximum possible total area of the pieces of paper in the garland Vasya wants to get or -1, if it is impossible to make the garland from the sheets he's got. It is guaranteed that the answer is always an integer.</p></div>

## Input

<p>The first line contains a non-empty sequence of <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) small English letters ("<span class="tex-font-style-tt">a</span>"<span class="tex-span">...</span>"<span class="tex-font-style-tt">z</span>"). Each letter means that Vasya has a sheet of paper of the corresponding color.</p><p>The second line contains a non-empty sequence of <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) small English letters that correspond to the colors of the pieces of paper in the garland that Vasya wants to make.</p>

## Output

<p>Print an integer that is the maximum possible total area of the pieces of paper in the garland Vasya wants to get or -1, if it is impossible to make the garland from the sheets he's got. It is guaranteed that the answer is always an integer.</p>





```input1
aaabbac
aabbccac

```




```input2
a
z

```




```output1
6

```




```output2
-1
```



## Note

<p>In the first test sample Vasya can make an garland of area 6: he can use both sheets of color <span class="tex-span"><i>b</i></span>, three (but not four) sheets of color <span class="tex-span"><i>a</i></span> and cut a single sheet of color <span class="tex-span"><i>c</i></span> in three, for example, equal pieces. Vasya can use the resulting pieces to make a garland of area 6.</p><p>In the second test sample Vasya cannot make a garland at all — he doesn't have a sheet of color <span class="tex-span"><i>z</i></span>.</p>
