## Description

<div><p>Several years ago Tolya had <span class="tex-span"><i>n</i></span> computer games and at some point of time he decided to burn them to CD. After that he wrote down the names of the games one after another in a circle on the CD <span class="tex-font-style-bf">in clockwise order</span>. The names were distinct, the length of each name was equal to <span class="tex-span"><i>k</i></span>. The names didn't overlap.</p><p>Thus, there is a cyclic string of length <span class="tex-span"><i>n</i>·<i>k</i></span> written on the CD.</p><p>Several years have passed and now Tolya can't remember which games he burned to his CD. He knows that there were <span class="tex-span"><i>g</i></span> popular games that days. All of the games he burned were among these <span class="tex-span"><i>g</i></span> games, and <span class="tex-font-style-bf">no game was burned more than once</span>.</p><p>You have to restore any valid list of games Tolya could burn to the CD several years ago.</p></div><div class="input-specification"><p>The first line of the input contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the amount of games Tolya burned to the CD, and the length of each of the names.</p><p>The second line of the input contains one string consisting of lowercase English letters&nbsp;— the string Tolya wrote on the CD, split in arbitrary place. The length of the string is <span class="tex-span"><i>n</i>·<i>k</i></span>. It is guaranteed that the length is not greater than <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>The third line of the input contains one positive integer <span class="tex-span"><i>g</i></span> (<span class="tex-span"><i>n</i> ≤ <i>g</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the amount of popular games that could be written on the CD. It is guaranteed that the total length of names of all popular games is not greater than <span class="tex-span">2·10<sup class="upper-index">6</sup></span>.</p><p>Each of the next <span class="tex-span"><i>g</i></span> lines contains a single string&nbsp;— the name of some popular game. Each name consists of lowercase English letters and has length <span class="tex-span"><i>k</i></span>. It is guaranteed that the names are distinct.</p></div><div class="output-specification"><p>If there is no answer, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, print two lines. In the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes). In the second line, print <span class="tex-span"><i>n</i></span> integers&nbsp;— the games which names were written on the CD. You should print games in the order they could have been written on the CD, it means, <span class="tex-font-style-bf">in clockwise order</span>. You can print games starting from any position. Remember, that no game was burned to the CD more than once. If there are several possible answers, print any of them.</p></div>

## Input

<p>The first line of the input contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the amount of games Tolya burned to the CD, and the length of each of the names.</p><p>The second line of the input contains one string consisting of lowercase English letters&nbsp;— the string Tolya wrote on the CD, split in arbitrary place. The length of the string is <span class="tex-span"><i>n</i>·<i>k</i></span>. It is guaranteed that the length is not greater than <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>The third line of the input contains one positive integer <span class="tex-span"><i>g</i></span> (<span class="tex-span"><i>n</i> ≤ <i>g</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the amount of popular games that could be written on the CD. It is guaranteed that the total length of names of all popular games is not greater than <span class="tex-span">2·10<sup class="upper-index">6</sup></span>.</p><p>Each of the next <span class="tex-span"><i>g</i></span> lines contains a single string&nbsp;— the name of some popular game. Each name consists of lowercase English letters and has length <span class="tex-span"><i>k</i></span>. It is guaranteed that the names are distinct.</p>

## Output

<p>If there is no answer, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, print two lines. In the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes). In the second line, print <span class="tex-span"><i>n</i></span> integers&nbsp;— the games which names were written on the CD. You should print games in the order they could have been written on the CD, it means, <span class="tex-font-style-bf">in clockwise order</span>. You can print games starting from any position. Remember, that no game was burned to the CD more than once. If there are several possible answers, print any of them.</p>





```input1
3 1
abc
4
b
a
c
d

```




```input2
4 2
aabbccdd
4
dd
ab
bc
cd

```




```output1
YES
2 1 3 

```




```output2
NO

```


