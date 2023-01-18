## Description

<div><p>As technologies develop, manufacturers are making the process of unlocking a phone as user-friendly as possible. To unlock its new phone, Arkady's pet dog Mu-mu has to bark the password once. The phone represents a password as a string of two lowercase English letters.</p><p>Mu-mu's enemy Kashtanka wants to unlock Mu-mu's phone to steal some sensible information, but it can only bark <span class="tex-span"><i>n</i></span> distinct words, each of which can be represented as a string of two lowercase English letters. Kashtanka wants to bark several words (not necessarily distinct) one after another to pronounce a string containing the password as a substring. Tell if it's possible to unlock the phone in this way, or not.</p></div><div class="input-specification"><p>The first line contains two lowercase English letters&nbsp;— the password on the phone.</p><p>The second line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of words Kashtanka knows.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain two lowercase English letters each, representing the words Kashtanka knows. The words are guaranteed to be distinct.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" if Kashtanka can bark several words in a line forming a string containing the password, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each letter in arbitrary case (upper or lower).</p></div>

## Input

<p>The first line contains two lowercase English letters&nbsp;— the password on the phone.</p><p>The second line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the number of words Kashtanka knows.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain two lowercase English letters each, representing the words Kashtanka knows. The words are guaranteed to be distinct.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" if Kashtanka can bark several words in a line forming a string containing the password, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can print each letter in arbitrary case (upper or lower).</p>





```input1
ya
4
ah
oy
to
ha

```




```input2
hp
2
ht
tp

```




```input3
ah
1
ha

```




```output1
YES

```




```output2
NO

```




```output3
YES

```



## Note

<p>In the first example the password is "<span class="tex-font-style-tt">ya</span>", and Kashtanka can bark "<span class="tex-font-style-tt">oy</span>" and then "<span class="tex-font-style-tt">ah</span>", and then "<span class="tex-font-style-tt">ha</span>" to form the string "<span class="tex-font-style-tt">oyahha</span>" which contains the password. So, the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the second example Kashtanka can't produce a string containing password as a substring. Note that it can bark "<span class="tex-font-style-tt">ht</span>" and then "<span class="tex-font-style-tt">tp</span>" producing "<span class="tex-font-style-tt">http</span>", but it doesn't contain the password "<span class="tex-font-style-tt">hp</span>" as a substring.</p><p>In the third example the string "<span class="tex-font-style-tt">hahahaha</span>" contains "<span class="tex-font-style-tt">ah</span>" as a substring.</p>
