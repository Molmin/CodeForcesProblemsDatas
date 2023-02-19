## Description

<div><p>Mahmoud wrote a message <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. He wants to send it as a birthday present to his friend Moaz who likes strings. He wrote it on a magical paper but he was surprised because some characters disappeared while writing the string. That's because this magical paper doesn't allow character number <span class="tex-span"><i>i</i></span> in the English alphabet to be written on it in a string of length more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. For example, if <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 2</span> he can't write character '<span class="tex-font-style-tt">a</span>' on this paper in a string of length <span class="tex-span">3</span> or more. String "<span class="tex-font-style-tt">aa</span>" is allowed while string "<span class="tex-font-style-tt">aaa</span>" is not.</p><p>Mahmoud decided to split the message into some non-empty substrings so that he can write every substring on an independent magical paper and fulfill the condition. The sum of their lengths should be <span class="tex-span"><i>n</i></span> and they shouldn't overlap. For example, if <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 2</span> and he wants to send string "<span class="tex-font-style-tt">aaa</span>", he can split it into "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">aa</span>" and use <span class="tex-span">2</span> magical papers, or into "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">a</span>" and use <span class="tex-span">3</span> magical papers. He can't split it into "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">aa</span>" because the sum of their lengths is greater than <span class="tex-span"><i>n</i></span>. He can split the message into single string if it fulfills the conditions.</p><p>A substring of string <span class="tex-span"><i>s</i></span> is a string that consists of some consecutive characters from string <span class="tex-span"><i>s</i></span>, strings "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">abc</span>" and "<span class="tex-font-style-tt">b</span>" are substrings of string "<span class="tex-font-style-tt">abc</span>", while strings "<span class="tex-font-style-tt">acb</span>" and "<span class="tex-font-style-tt">ac</span>" are not. Any string is a substring of itself.</p><p>While Mahmoud was thinking of how to split the message, Ehab told him that there are many ways to split it. After that Mahmoud asked you three questions: </p><ul> <li> How many ways are there to split the string into substrings such that every substring fulfills the condition of the magical paper, the sum of their lengths is <span class="tex-span"><i>n</i></span> and they don't overlap? Compute the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. </li><li> What is the maximum length of a substring that can appear in some valid splitting? </li><li> What is the minimum number of substrings the message can be spit in? </li></ul><p>Two ways are considered different, if the sets of split positions differ. For example, splitting "<span class="tex-font-style-tt">aa|a</span>" and "<span class="tex-font-style-tt">a|aa</span>" are considered different splittings of message "<span class="tex-font-style-tt">aaa</span>".</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) denoting the length of the message.</p><p>The second line contains the message <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> that consists of lowercase English letters.</p><p>The third line contains <span class="tex-span">26</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">26</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>x</i></sub> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the maximum lengths of substring each letter can appear in.</p></div><div class="output-specification"><p>Print three lines.</p><p>In the first line print the number of ways to split the message into substrings and fulfill the conditions mentioned in the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup>  +  7</span>.</p><p>In the second line print the length of the longest substring over all the ways.</p><p>In the third line print the minimum number of substrings over all the ways.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">3</sup></span>) denoting the length of the message.</p><p>The second line contains the message <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> that consists of lowercase English letters.</p><p>The third line contains <span class="tex-span">26</span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index">26</sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>x</i></sub> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— the maximum lengths of substring each letter can appear in.</p>

## Output

<p>Print three lines.</p><p>In the first line print the number of ways to split the message into substrings and fulfill the conditions mentioned in the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup>  +  7</span>.</p><p>In the second line print the length of the longest substring over all the ways.</p><p>In the third line print the minimum number of substrings over all the ways.</p>





```input1
3
aab
2 3 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1

```




```input2
10
abcdeabcde
5 5 5 5 4 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1

```




```output1
3
2
2

```




```output2
401
4
3

```



## Note

<p>In the first example the three ways to split the message are: </p><ul> <li> <span class="tex-font-style-tt">a|a|b</span> </li><li> <span class="tex-font-style-tt">aa|b</span> </li><li> <span class="tex-font-style-tt">a|ab</span> </li></ul><p>The longest substrings are "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">ab</span>" of length <span class="tex-span">2</span>.</p><p>The minimum number of substrings is <span class="tex-span">2</span> in "<span class="tex-font-style-tt">a|ab</span>" or "<span class="tex-font-style-tt">aa|b</span>".</p><p>Notice that "<span class="tex-font-style-tt">aab</span>" is not a possible splitting because the letter '<span class="tex-font-style-tt">a</span>' appears in a substring of length <span class="tex-span">3</span>, while <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = 2</span>.</p>
