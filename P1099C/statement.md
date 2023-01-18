## Description

<div><p>Andrey received a postcard from Irina. It contained only the words "Hello, Andrey!", and a strange string consisting of lowercase Latin letters, snowflakes and candy canes. Andrey thought that this string is an encrypted message, and decided to decrypt it.</p><p>Andrey noticed that snowflakes and candy canes always stand after the letters, so he supposed that the message was encrypted as follows. Candy cane means that the letter before it can be removed, or can be left. A snowflake means that the letter before it can be removed, left, or repeated several times.</p><p>For example, consider the following string: </p><center> <img class="tex-graphics" src="file://bFxHNDxl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>This string can encode the message «<span class="tex-font-style-tt">happynewyear</span>». For this, candy canes and snowflakes should be used as follows: </p><ul> <li> candy cane 1: remove the letter <span class="tex-font-style-tt">w</span>, </li><li> snowflake 1: repeat the letter <span class="tex-font-style-tt">p</span> twice, </li><li> candy cane 2: leave the letter <span class="tex-font-style-tt">n</span>, </li><li> snowflake 2: remove the letter <span class="tex-font-style-tt">w</span>, </li><li> snowflake 3: leave the letter <span class="tex-font-style-tt">e</span>. </li></ul><center> <img class="tex-graphics" src="file://2swdZ08a.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Please note that the same string can encode different messages. For example, the string above can encode «<span class="tex-font-style-tt">hayewyar</span>», «<span class="tex-font-style-tt">happpppynewwwwwyear</span>», and other messages.</p><p>Andrey knows that messages from Irina usually have a length of $k$ letters. Help him to find out if a given string can encode a message of $k$ letters, and if so, give an example of such a message.</p></div><div class="input-specification"><p>The first line contains the string received in the postcard. The string consists only of lowercase Latin letters, as well as the characters «<span class="tex-font-style-tt">*</span>» and «<span class="tex-font-style-tt">?</span>», meaning snowflake and candy cone, respectively. These characters can only appear immediately after the letter. The length of the string does not exceed $200$.</p><p>The second line contains an integer number $k$ ($1 \leq k \leq 200$), the required message length.</p></div><div class="output-specification"><p>Print any message of length $k$ that the given string can encode, or «<span class="tex-font-style-tt">Impossible</span>» if such a message does not exist.</p></div>

## Input

<p>The first line contains the string received in the postcard. The string consists only of lowercase Latin letters, as well as the characters «<span class="tex-font-style-tt">*</span>» and «<span class="tex-font-style-tt">?</span>», meaning snowflake and candy cone, respectively. These characters can only appear immediately after the letter. The length of the string does not exceed $200$.</p><p>The second line contains an integer number $k$ ($1 \leq k \leq 200$), the required message length.</p>

## Output

<p>Print any message of length $k$ that the given string can encode, or «<span class="tex-font-style-tt">Impossible</span>» if such a message does not exist.</p>





```input1
hw?ap*yn?eww*ye*ar
12
```




```input2
ab?a
2
```




```input3
ab?a
3
```




```input4
ababb
5
```




```input5
ab?a
1
```




```output1
happynewyear
```




```output2
aa
```




```output3
aba
```




```output4
ababb
```




```output5
Impossible
```


