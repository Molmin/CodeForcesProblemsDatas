## Description

<div><p>You have probably registered on Internet sites many times. And each time you should enter your invented password. Usually the registration form automatically checks the password's crypt resistance. If the user's password isn't complex enough, a message is displayed. Today your task is to implement such an automatic check.</p><p>Web-developers of the company Q assume that a password is complex enough, if it meets all of the following conditions:</p><ul> <li> the password length is at least 5 characters; </li><li> the password contains at least one large English letter; </li><li> the password contains at least one small English letter; </li><li> the password contains at least one digit. </li></ul><p>You are given a password. Please implement the automatic check of its complexity for company Q.</p></div><div class="input-specification"><p>The first line contains a non-empty sequence of characters (at most <span class="tex-span">100</span> characters). Each character is either a large English letter, or a small English letter, or a digit, or one of characters: "<span class="tex-font-style-tt">!</span>", "<span class="tex-font-style-tt">?</span>", "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">,</span>", "<span class="tex-font-style-tt">_</span>".</p></div><div class="output-specification"><p>If the password is complex enough, print message "<span class="tex-font-style-tt">Correct</span>" (without the quotes), otherwise print message "<span class="tex-font-style-tt">Too weak</span>" (without the quotes).</p></div>

## Input

<p>The first line contains a non-empty sequence of characters (at most <span class="tex-span">100</span> characters). Each character is either a large English letter, or a small English letter, or a digit, or one of characters: "<span class="tex-font-style-tt">!</span>", "<span class="tex-font-style-tt">?</span>", "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">,</span>", "<span class="tex-font-style-tt">_</span>".</p>

## Output

<p>If the password is complex enough, print message "<span class="tex-font-style-tt">Correct</span>" (without the quotes), otherwise print message "<span class="tex-font-style-tt">Too weak</span>" (without the quotes).</p>





```input1
abacaba

```




```input2
X12345

```




```input3
CONTEST_is_STARTED!!11

```




```output1
Too weak

```




```output2
Too weak

```




```output3
Correct

```


