## Description

<div><p>Those days, many boys use beautiful girls' photos as avatars in forums. So it is pretty hard to tell the gender of a user at the first glance. Last year, our hero went to a forum and had a nice chat with a beauty (he thought so). After that they talked very often and eventually they became a couple in the network. </p><p>But yesterday, he came to see "her" in the real world and found out "she" is actually a very strong man! Our hero is very sad and he is too tired to love again now. So he came up with a way to recognize users' genders by their user names.</p><p>This is his method: if the number of distinct characters in one's user name is odd, then he is a male, otherwise she is a female. You are given the string that denotes the user name, please help our hero to determine the gender of this user by his method.</p></div><div class="input-specification"><p>The first line contains a non-empty string, that contains only lowercase English letters — the user name. This string contains at most 100 letters.</p></div><div class="output-specification"><p>If it is a female by our hero's method, print "<span class="tex-font-style-tt">CHAT WITH HER!</span>" (without the quotes), otherwise, print "<span class="tex-font-style-tt">IGNORE HIM!</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a non-empty string, that contains only lowercase English letters — the user name. This string contains at most 100 letters.</p>

## Output

<p>If it is a female by our hero's method, print "<span class="tex-font-style-tt">CHAT WITH HER!</span>" (without the quotes), otherwise, print "<span class="tex-font-style-tt">IGNORE HIM!</span>" (without the quotes).</p>





```input1
wjmzbmr

```




```input2
xiaodao

```




```input3
sevenkplus

```




```output1
CHAT WITH HER!

```




```output2
IGNORE HIM!

```




```output3
CHAT WITH HER!

```



## Note

<p>For the first example. There are 6 distinct characters in "<span class="tex-font-style-tt">wjmzbmr</span>". These characters are: "<span class="tex-font-style-tt">w</span>", "<span class="tex-font-style-tt">j</span>", "<span class="tex-font-style-tt">m</span>", "<span class="tex-font-style-tt">z</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">r</span>". So wjmzbmr is a female and you should print "<span class="tex-font-style-tt">CHAT WITH HER!</span>".</p>
