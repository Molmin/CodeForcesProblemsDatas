## Description

<div><p>When registering in a social network, users are allowed to create their own convenient login to make it easier to share contacts, print it on business cards, etc.</p><p>Login is an arbitrary sequence of lower and uppercase latin letters, digits and underline symbols («<span class="tex-font-style-tt">_</span>»). However, in order to decrease the number of frauds and user-inattention related issues, it is prohibited to register a login if it is <span class="tex-font-style-it">similar</span> with an already existing login. More precisely, two logins <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are considered similar if we can transform <span class="tex-span"><i>s</i></span> to <span class="tex-span"><i>t</i></span> via a sequence of operations of the following types: </p><ul> <li> transform lowercase letters to uppercase and vice versa; </li><li> change letter «<span class="tex-font-style-tt">O</span>» (uppercase latin letter) to digit «<span class="tex-font-style-tt">0</span>» and vice versa; </li><li> change digit «<span class="tex-font-style-tt">1</span>» (one) to any letter among «<span class="tex-font-style-tt">l</span>» (lowercase latin «<span class="tex-font-style-tt">L</span>»), «<span class="tex-font-style-tt">I</span>» (uppercase latin «<span class="tex-font-style-tt">i</span>») and vice versa, or change one of these letters to other. </li></ul><p>For example, logins «<span class="tex-font-style-tt">Codeforces</span>» and «<span class="tex-font-style-tt">codef0rces</span>» as well as «<span class="tex-font-style-tt">OO0OOO00O0OOO0O00OOO0OO_lol</span>» and «<span class="tex-font-style-tt">OO0OOO0O00OOO0O00OO0OOO_1oI</span>» are considered similar whereas «<span class="tex-font-style-tt">Codeforces</span>» and «<span class="tex-font-style-tt">Code_forces</span>» are not.</p><p>You're given a list of existing logins with no two <span class="tex-font-style-it">similar</span> amonst and a newly created user login. Check whether this new login is <span class="tex-font-style-it">similar</span> with any of the existing ones.</p></div><div class="input-specification"><p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of lower and uppercase latin letters, digits and underline symbols («<span class="tex-font-style-tt">_</span>») with length not exceeding <span class="tex-span">50</span> &nbsp;— the login itself.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>)&nbsp;— the number of existing logins.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the existing logins, following the same constraints as the user login (refer to the first line of the input). It's guaranteed that no two existing logins are similar.</p></div><div class="output-specification"><p>Print «<span class="tex-font-style-tt">Yes</span>» (without quotes), if user can register via this login, i.e. none of the existing logins is <span class="tex-font-style-it">similar</span> with it.</p><p>Otherwise print «<span class="tex-font-style-tt">No</span>» (without quotes).</p></div>

## Input

<p>The first line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of lower and uppercase latin letters, digits and underline symbols («<span class="tex-font-style-tt">_</span>») with length not exceeding <span class="tex-span">50</span> &nbsp;— the login itself.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>)&nbsp;— the number of existing logins.</p><p>The next <span class="tex-span"><i>n</i></span> lines describe the existing logins, following the same constraints as the user login (refer to the first line of the input). It's guaranteed that no two existing logins are similar.</p>

## Output

<p>Print «<span class="tex-font-style-tt">Yes</span>» (without quotes), if user can register via this login, i.e. none of the existing logins is <span class="tex-font-style-it">similar</span> with it.</p><p>Otherwise print «<span class="tex-font-style-tt">No</span>» (without quotes).</p>





```input1
1_wat
2
2_wat
wat_1

```




```input2
000
3
00
ooA
oOo

```




```input3
_i_
3
__i_
_1_
I

```




```input4
La0
3
2a0
La1
1a0

```




```input5
abc
1
aBc

```




```input6
0Lil
2
LIL0
0Ril

```




```output1
Yes

```




```output2
No

```




```output3
No

```




```output4
No

```




```output5
No

```




```output6
Yes

```



## Note

<p>In the second sample case the user wants to create a login consisting of three zeros. It's impossible due to collision with the third among the existing.</p><p>In the third sample case the new login is similar with the second one.</p>
