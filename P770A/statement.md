## Description

<div><p>Innokentiy decides to change the password in the social net "Contact!", but he is too lazy to invent a new password by himself. That is why he needs your help. </p><p>Innokentiy decides that new password should satisfy the following conditions:</p><ul> <li> the length of the password must be equal to <span class="tex-span"><i>n</i></span>, </li><li> the password should consist only of lowercase Latin letters, </li><li> the number of distinct symbols in the password must be equal to <span class="tex-span"><i>k</i></span>, </li><li> any two consecutive symbols in the password must be distinct. </li></ul><p>Your task is to help Innokentiy and to invent a new password which will satisfy all given conditions. </p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 26)</span>) — the length of the password and the number of distinct symbols in it. </p><p>Pay attention that a desired new password always exists.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-bf">any</span> password which satisfies all conditions given by Innokentiy.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>k</i> ≤ <i>min</i>(<i>n</i>, 26)</span>) — the length of the password and the number of distinct symbols in it. </p><p>Pay attention that a desired new password always exists.</p>

## Output

<p>Print <span class="tex-font-style-bf">any</span> password which satisfies all conditions given by Innokentiy.</p>





```input1
4 3

```




```input2
6 6

```




```input3
5 2

```




```output1
java

```




```output2
python

```




```output3
phphp

```



## Note

<p>In the first test there is one of the appropriate new passwords — <span class="tex-font-style-tt">java</span>, because its length is equal to <span class="tex-span">4</span> and <span class="tex-span">3</span> distinct lowercase letters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">j</span> and <span class="tex-font-style-tt">v</span> are used in it.</p><p>In the second test there is one of the appropriate new passwords — <span class="tex-font-style-tt">python</span>, because its length is equal to <span class="tex-span">6</span> and it consists of <span class="tex-span">6</span> distinct lowercase letters.</p><p>In the third test there is one of the appropriate new passwords — <span class="tex-font-style-tt">phphp</span>, because its length is equal to <span class="tex-span">5</span> and <span class="tex-span">2</span> distinct lowercase letters <span class="tex-font-style-tt">p</span> and <span class="tex-font-style-tt">h</span> are used in it.</p><p>Pay attention the condition that no two identical symbols are consecutive is correct for all appropriate passwords in tests. </p>
