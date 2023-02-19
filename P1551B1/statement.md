## Description

<div><p><span class="tex-font-style-it">This is a simplified version of the problem B2. Perhaps you should read the problem B2 before you start solving B1.</span></p><p>Paul and Mary have a favorite string $s$ which consists of lowercase letters of the Latin alphabet. They want to paint it using pieces of chalk of two colors: red and green. Let's call a coloring of a string wonderful if the following conditions are met:</p><ol> <li> each letter of the string is either painted in exactly one color (red or green) or isn't painted; </li><li> each two letters which are painted in the same color are different; </li><li> the number of letters painted in red is equal to the number of letters painted in green; </li><li> the number of painted letters of this coloring is <span class="tex-font-style-bf">maximum</span> among all colorings of the string which meet the first three conditions. </li></ol><p>E. g. consider a string $s$ equal to "<span class="tex-font-style-tt">kzaaa</span>". One of the wonderful colorings of the string is shown in the figure.</p><center> <img class="tex-graphics" src="file://JSTIIyRS.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-small">The example of a wonderful coloring of the string "<span class="tex-font-style-tt">kzaaa</span>".</span> </center><p>Paul and Mary want to learn by themselves how to find a wonderful coloring of the string. But they are very young, so they need a hint. Help them find $k$ — the number of red (or green, these numbers are equal) letters in a wonderful coloring.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one non-empty string $s$ which consists of lowercase letters of the Latin alphabet. The number of characters in the string doesn't exceed $50$.</p></div><div class="output-specification"><p>For each test case, output a separate line containing one non-negative integer $k$ — the number of letters which will be painted in red in a wonderful coloring.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 1000$) — the number of test cases. Then $t$ test cases follow.</p><p>Each test case consists of one non-empty string $s$ which consists of lowercase letters of the Latin alphabet. The number of characters in the string doesn't exceed $50$.</p>

## Output

<p>For each test case, output a separate line containing one non-negative integer $k$ — the number of letters which will be painted in red in a wonderful coloring.</p>





```input1
5
kzaaa
codeforces
archive
y
xxxxxx
```




```output1
2
5
3
0
1
```



## Note

<p>The first test case contains the string from the statement. One of the wonderful colorings is shown in the figure. There's no wonderful coloring containing $3$ or more red letters because the total number of painted symbols will exceed the string's length.</p><p>The string from the second test case can be painted as follows. Let's paint the first occurrence of each of the letters "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">o</span>", "<span class="tex-font-style-tt">e</span>" in red and the second ones in green. Let's paint the letters "<span class="tex-font-style-tt">d</span>", "<span class="tex-font-style-tt">f</span>" in red and "<span class="tex-font-style-tt">r</span>", "<span class="tex-font-style-tt">s</span>" in green. So every letter will be painted in red or green, hence the answer better than $5$ doesn't exist.</p><p>The third test case contains the string of distinct letters, so you can paint any set of characters in red, as long as the size of this set doesn't exceed half of the size of the string and is the maximum possible.</p><p>The fourth test case contains a single letter which cannot be painted in red because there will be no letter able to be painted in green.</p><p>The fifth test case contains a string of identical letters, so there's no way to paint more than one letter in red.</p>
