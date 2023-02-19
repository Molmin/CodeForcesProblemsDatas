## Description

<div><p>After overcoming the stairs Dasha came to classes. She needed to write a password to begin her classes. The password is a string of length <span class="tex-span"><i>n</i></span> which satisfies the following requirements:</p><ul> <li> There is at least one digit in the string, </li><li> There is at least one lowercase (small) letter of the Latin alphabet in the string, </li><li> There is at least one of three listed symbols in the string: '<span class="tex-font-style-tt">#</span>', '<span class="tex-font-style-tt">*</span>', '<span class="tex-font-style-tt">&amp;</span>'. </li></ul><center> <img class="tex-graphics" src="file://xEE2FKeH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Considering that these are programming classes it is not easy to write the password.</p><p>For each character of the password we have a fixed string of length <span class="tex-span"><i>m</i></span>, on each of these <span class="tex-span"><i>n</i></span> strings there is a pointer on some character. The <span class="tex-span"><i>i</i></span>-th character displayed on the screen is the pointed character in the <span class="tex-span"><i>i</i></span>-th string. Initially, all pointers are on characters with indexes <span class="tex-span">1</span> in the corresponding strings (all positions are numbered starting from one).</p><p>During one operation Dasha can move a pointer in one string one character to the left or to the right. Strings are cyclic, it means that when we move the pointer which is on the character with index <span class="tex-span">1</span> to the left, it moves to the character with the index <span class="tex-span"><i>m</i></span>, and when we move it to the right from the position <span class="tex-span"><i>m</i></span> it moves to the position <span class="tex-span">1</span>.</p><p>You need to determine the minimum number of operations necessary to make the string displayed on the screen a valid password. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 50, 1 ≤ <i>m</i> ≤ 50)</span> — the length of the password and the length of strings which are assigned to password symbols. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains the string which is assigned to the <span class="tex-span"><i>i</i></span>-th symbol of the password string. Its length is <span class="tex-span"><i>m</i></span>, it consists of digits, lowercase English letters, and characters '<span class="tex-font-style-tt">#</span>', '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">&amp;</span>'.</p><p>You have such input data that you can always get a valid password.</p></div><div class="output-specification"><p>Print one integer — the minimum number of operations which is necessary to make the string, which is displayed on the screen, a valid password. </p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(3 ≤ <i>n</i> ≤ 50, 1 ≤ <i>m</i> ≤ 50)</span> — the length of the password and the length of strings which are assigned to password symbols. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains the string which is assigned to the <span class="tex-span"><i>i</i></span>-th symbol of the password string. Its length is <span class="tex-span"><i>m</i></span>, it consists of digits, lowercase English letters, and characters '<span class="tex-font-style-tt">#</span>', '<span class="tex-font-style-tt">*</span>' or '<span class="tex-font-style-tt">&amp;</span>'.</p><p>You have such input data that you can always get a valid password.</p>

## Output

<p>Print one integer — the minimum number of operations which is necessary to make the string, which is displayed on the screen, a valid password. </p>





```input1
3 4
1**2
a3*0
c4**

```




```input2
5 5
#*&amp;#*
*a1c&amp;
&amp;q2w*
#a3c#
*&amp;#*&amp;

```




```output1
1

```




```output2
3

```



## Note

<p>In the first test it is necessary to move the pointer of the third string to one left to get the optimal answer. </p><center> <img class="tex-graphics" src="file://oyN32RXo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second test one of possible algorithms will be: </p><ul> <li> to move the pointer of the second symbol once to the right. </li><li> to move the pointer of the third symbol twice to the right. </li></ul><center> <img class="tex-graphics" src="file://KVynDpq7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
