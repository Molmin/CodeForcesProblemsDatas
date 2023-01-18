## Description

<div><p>Nam is playing with a string on his computer. The string consists of <span class="tex-span"><i>n</i></span> lowercase English letters. It is meaningless, so Nam decided to make the string more beautiful, that is to make it be a palindrome by using 4 arrow keys: left, right, up, down.</p><p>There is a cursor pointing at some symbol of the string. Suppose that cursor is at position <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, the string uses 1-based indexing) now. Left and right arrow keys are used to move cursor around the string. The string is cyclic, that means that when Nam presses left arrow key, the cursor will move to position <span class="tex-span"><i>i</i> - 1</span> if <span class="tex-span"><i>i</i> &gt; 1</span> or to the end of the string (i. e. position <span class="tex-span"><i>n</i></span>) otherwise. The same holds when he presses the right arrow key (if <span class="tex-span"><i>i</i> = <i>n</i></span>, the cursor appears at the beginning of the string).</p><p>When Nam presses up arrow key, the letter which the text cursor is pointing to will change to the next letter in English alphabet (assuming that alphabet is also cyclic, i. e. after '<span class="tex-font-style-tt">z</span>' follows '<span class="tex-font-style-tt">a</span>'). The same holds when he presses the down arrow key.</p><p>Initially, the text cursor is at position <span class="tex-span"><i>p</i></span>. </p><p>Because Nam has a lot homework to do, he wants to complete this as fast as possible. Can you help him by calculating the minimum number of arrow keys presses to make the string to be a palindrome?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>), the length of Nam's string and the initial position of the text cursor.</p><p>The next line contains <span class="tex-span"><i>n</i></span> lowercase characters of Nam's string.</p></div><div class="output-specification"><p>Print the minimum number of presses needed to change string into a palindrome.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ <i>n</i></span>), the length of Nam's string and the initial position of the text cursor.</p><p>The next line contains <span class="tex-span"><i>n</i></span> lowercase characters of Nam's string.</p>

## Output

<p>Print the minimum number of presses needed to change string into a palindrome.</p>





```input1
8 3
aeabcaez

```




```output1
6

```



## Note

<p>A string is a palindrome if it reads the same forward or reversed.</p><p>In the sample test, initial Nam's string is: <img align="middle" class="tex-formula" src="file://sg4esG37.png" style="max-width: 100.0%;max-height: 100.0%;"> (cursor position is shown bold).</p><p>In optimal solution, Nam may do <span class="tex-span">6</span> following steps:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://gSNMvpDI.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The result, <img align="middle" class="tex-formula" src="file://yOXoYNBe.png" style="max-width: 100.0%;max-height: 100.0%;">, is now a palindrome.</p>
