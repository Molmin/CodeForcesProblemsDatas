## Description

<div><p>There are a lot of rumors in the media these days. One day Aida decided to find out how rumors are made.</p><p>She asked <span class="tex-span"><i>n</i></span> of her friends to help her. They all formed a circle and Aida told the person to her right a piece of news which was just a simple string. Then each person told the string to the person on his/her right. But they didn't tell the string exactly as they'd heard it. Each person made <span class="tex-font-style-underline">at most</span> one of these two types of changes: </p><ul> <li> Removing one character from the end of the heard string. </li><li> Adding a character to the end of the heard string. </li></ul><p>Finally when the rumor passed exactly <span class="tex-span"><i>n</i></span> moves (a complete cycle), Aida heard something quite different from what she expected from the person on her left. She thinks someone has cheated and made some changes other than those explained above. Now she wants you to write a <span class="tex-font-style-underline">Pike</span> piece of code which gets the initial and final strings and tells Aida whether it's possible to get to the final string from the initial one, by the rules described above.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 8 × 10<sup class="upper-index">6</sup></span>), the number of Aida's friends. The following two lines contain a <span class="tex-font-style-underline">non-empty</span> string each — initial and final strings. The lengths of strings are at most <span class="tex-span">10<sup class="upper-index">7</sup></span> and they only contain English alphabet letters.</p></div><div class="output-specification"><p>Write a single <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span>. Write <span class="tex-font-style-tt">YES</span> only if it's possible to get to the final string from the initial string.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 8 × 10<sup class="upper-index">6</sup></span>), the number of Aida's friends. The following two lines contain a <span class="tex-font-style-underline">non-empty</span> string each — initial and final strings. The lengths of strings are at most <span class="tex-span">10<sup class="upper-index">7</sup></span> and they only contain English alphabet letters.</p>

## Output

<p>Write a single <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span>. Write <span class="tex-font-style-tt">YES</span> only if it's possible to get to the final string from the initial string.</p>





```input1
100
Codeforces
MMIODPC

```




```input2
5
MMIOD
CF

```




```output1
Yes

```




```output2
No

```



## Note

<p>The input is case-sensitive, while the output is not.</p>
