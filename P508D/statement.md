## Description

<div><p>While dad was at work, a little girl Tanya decided to play with dad's password to his secret database. Dad's password is a string consisting of <span class="tex-span"><i>n</i> + 2</span> characters. She has written all the possible <span class="tex-span"><i>n</i></span> three-letter continuous substrings of the password on pieces of paper, one for each piece of paper, and threw the password out. Each three-letter substring was written the number of times it occurred in the password. Thus, Tanya ended up with <span class="tex-span"><i>n</i></span> pieces of paper.</p><p>Then Tanya realized that dad will be upset to learn about her game and decided to restore the password or at least any string corresponding to the final set of three-letter strings. You have to help her in this difficult task. We know that dad's password consisted of lowercase and uppercase letters of the Latin alphabet and digits. Uppercase and lowercase letters of the Latin alphabet are considered distinct.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>), the number of three-letter substrings Tanya got. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain three letters each, forming the substring of dad's password. Each character in the input is a lowercase or uppercase Latin letter or a digit.</p></div><div class="output-specification"><p>If Tanya made a mistake somewhere during the game and the strings that correspond to the given set of substrings don't exist, print "<span class="tex-font-style-tt">NO</span>". </p><p>If it is possible to restore the string that corresponds to given set of substrings, print "<span class="tex-font-style-tt">YES</span>", and then print any suitable password option.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>), the number of three-letter substrings Tanya got. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain three letters each, forming the substring of dad's password. Each character in the input is a lowercase or uppercase Latin letter or a digit.</p>

## Output

<p>If Tanya made a mistake somewhere during the game and the strings that correspond to the given set of substrings don't exist, print "<span class="tex-font-style-tt">NO</span>". </p><p>If it is possible to restore the string that corresponds to given set of substrings, print "<span class="tex-font-style-tt">YES</span>", and then print any suitable password option.</p>





```input1
5
aca
aba
aba
cab
bac

```




```input2
4
abc
bCb
cb1
b13

```




```input3
7
aaa
aaa
aaa
aaa
aaa
aaa
aaa

```




```output1
YES
abacaba

```




```output2
NO

```




```output3
YES
aaaaaaaaa

```


