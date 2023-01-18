## Description

<div><p>A large banner with word <span class="tex-font-style-tt">CODEFORCES</span> was ordered for the 1000-th onsite round of Codeforces<span class="tex-span"><sup class="upper-index">ω</sup></span> that takes place on the Miami beach. Unfortunately, the company that made the banner mixed up two orders and delivered somebody else's banner that contains someone else's word. The word on the banner consists only of upper-case English letters.</p><p>There is very little time to correct the mistake. All that we can manage to do is to cut out some <span class="tex-font-style-it">substring</span> from the banner, i.e. several consecutive letters. After that all the resulting parts of the banner will be glued into a single piece (if the beginning or the end of the original banner was cut out, only one part remains); it is not allowed change the relative order of parts of the banner (i.e. after a substring is cut, several first and last letters are left, it is allowed only to glue the last letters to the right of the first letters). Thus, for example, for example, you can cut a substring out from string '<span class="tex-font-style-tt">TEMPLATE</span>' and get string '<span class="tex-font-style-tt">TEMPLE</span>' (if you cut out string <span class="tex-font-style-tt">AT</span>), '<span class="tex-font-style-tt">PLATE</span>' (if you cut out <span class="tex-font-style-tt">TEM</span>), '<span class="tex-font-style-tt">T</span>' (if you cut out <span class="tex-font-style-tt">EMPLATE</span>), etc.</p><p>Help the organizers of the round determine whether it is possible to cut out of the banner some substring in such a way that the remaining parts formed word <span class="tex-font-style-tt">CODEFORCES</span>.</p></div><div class="input-specification"><p>The single line of the input contains the word written on the banner. The word only consists of upper-case English letters. The word is non-empty and its length doesn't exceed 100 characters. It is guaranteed that the word isn't word <span class="tex-font-style-tt">CODEFORCES</span>.</p></div><div class="output-specification"><p>Print '<span class="tex-font-style-tt">YES</span>', if there exists a way to cut out the substring, and '<span class="tex-font-style-tt">NO</span>' otherwise (without the quotes).</p></div>

## Input

<p>The single line of the input contains the word written on the banner. The word only consists of upper-case English letters. The word is non-empty and its length doesn't exceed 100 characters. It is guaranteed that the word isn't word <span class="tex-font-style-tt">CODEFORCES</span>.</p>

## Output

<p>Print '<span class="tex-font-style-tt">YES</span>', if there exists a way to cut out the substring, and '<span class="tex-font-style-tt">NO</span>' otherwise (without the quotes).</p>





```input1
CODEWAITFORITFORCES

```




```input2
BOTTOMCODER

```




```input3
DECODEFORCES

```




```input4
DOGEFORCES

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




```output4
NO

```


