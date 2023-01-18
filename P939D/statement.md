## Description

<div><p>Valya and Tolya are an ideal pair, but they quarrel sometimes. Recently, Valya took offense at her boyfriend because he came to her in t-shirt with lettering that differs from lettering on her pullover. Now she doesn't want to see him and Tolya is seating at his room and crying at her photos all day long.</p><p>This story could be very sad but fairy godmother (Tolya's grandmother) decided to help them and restore their relationship. She secretly took Tolya's t-shirt and Valya's pullover and wants to make the letterings on them same. In order to do this, for one unit of mana she can buy a spell that can change some letters on the clothes. Your task is calculate the minimum amount of mana that Tolya's grandmother should spend to rescue love of Tolya and Valya.</p><p>More formally, letterings on Tolya's t-shirt and Valya's pullover are two strings with same length <span class="tex-span"><i>n</i></span> consisting only of lowercase English letters. Using one unit of mana, grandmother can buy a spell of form <span class="tex-span">(<i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>)</span> (where <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> are some lowercase English letters), which can arbitrary number of times transform a single letter <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> to <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> and vise-versa on both Tolya's t-shirt and Valya's pullover. You should find the minimum amount of mana that grandmother should spend to buy a set of spells that can make the letterings equal. In addition you should output the required set of spells. </p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the letterings.</p><p>The second line contains a string with length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters&nbsp;— the lettering on Valya's pullover.</p><p>The third line contains the lettering on Tolya's t-shirt in the same format.</p></div><div class="output-specification"><p>In the first line output a single integer&nbsp;— the minimum amount of mana <span class="tex-span"><i>t</i></span> required for rescuing love of Valya and Tolya.</p><p>In the next <span class="tex-span"><i>t</i></span> lines output pairs of space-separated lowercase English letters&nbsp;— spells that Tolya's grandmother should buy. Spells and letters in spells can be printed in any order.</p><p>If there are many optimal answers, output any.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the letterings.</p><p>The second line contains a string with length <span class="tex-span"><i>n</i></span>, consisting of lowercase English letters&nbsp;— the lettering on Valya's pullover.</p><p>The third line contains the lettering on Tolya's t-shirt in the same format.</p>

## Output

<p>In the first line output a single integer&nbsp;— the minimum amount of mana <span class="tex-span"><i>t</i></span> required for rescuing love of Valya and Tolya.</p><p>In the next <span class="tex-span"><i>t</i></span> lines output pairs of space-separated lowercase English letters&nbsp;— spells that Tolya's grandmother should buy. Spells and letters in spells can be printed in any order.</p><p>If there are many optimal answers, output any.</p>





```input1
3
abb
dad

```




```input2
8
drpepper
cocacola

```




```output1
2
a d
b a
```




```output2
7
l e
e d
d c
c p
p o
o r
r a

```



## Note

<p>In first example it's enough to buy two spells: ('<span class="tex-font-style-tt">a</span>','<span class="tex-font-style-tt">d</span>') and ('<span class="tex-font-style-tt">b</span>','<span class="tex-font-style-tt">a</span>'). Then first letters will coincide when we will replace letter '<span class="tex-font-style-tt">a</span>' with '<span class="tex-font-style-tt">d</span>'. Second letters will coincide when we will replace '<span class="tex-font-style-tt">b</span>' with '<span class="tex-font-style-tt">a</span>'. Third letters will coincide when we will at first replace '<span class="tex-font-style-tt">b</span>' with '<span class="tex-font-style-tt">a</span>' and then '<span class="tex-font-style-tt">a</span>' with '<span class="tex-font-style-tt">d</span>'.</p>
