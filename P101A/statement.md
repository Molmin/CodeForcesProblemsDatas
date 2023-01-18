## Description

<div><p>Once when Gerald studied in the first year at school, his teacher gave the class the following homework. She offered the students a string consisting of <span class="tex-span"><i>n</i></span> small Latin letters; the task was to learn the way the letters that the string contains are written. However, as Gerald is too lazy, he has no desire whatsoever to learn those letters. That's why he decided to lose some part of the string (not necessarily a connected part). The lost part can consist of any number of segments of any length, at any distance from each other. However, Gerald knows that if he loses more than <span class="tex-span"><i>k</i></span> characters, it will be very suspicious. </p><p>Find the least number of distinct characters that can remain in the string after no more than <span class="tex-span"><i>k</i></span> characters are deleted. You also have to find any possible way to delete the characters.</p></div><div class="input-specification"><p>The first input data line contains a string whose length is equal to <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The string consists of lowercase Latin letters. The second line contains the number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print on the first line the only number <span class="tex-span"><i>m</i></span> — the least possible number of different characters that could remain in the given string after it loses no more than <span class="tex-span"><i>k</i></span> characters.</p><p>Print on the second line the string that Gerald can get after some characters are lost. The string should have exactly <span class="tex-span"><i>m</i></span> distinct characters. The final string should be the subsequence of the initial string. If Gerald can get several different strings with exactly <span class="tex-span"><i>m</i></span> distinct characters, print any of them.</p></div>

## Input

<p>The first input data line contains a string whose length is equal to <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The string consists of lowercase Latin letters. The second line contains the number <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print on the first line the only number <span class="tex-span"><i>m</i></span> — the least possible number of different characters that could remain in the given string after it loses no more than <span class="tex-span"><i>k</i></span> characters.</p><p>Print on the second line the string that Gerald can get after some characters are lost. The string should have exactly <span class="tex-span"><i>m</i></span> distinct characters. The final string should be the subsequence of the initial string. If Gerald can get several different strings with exactly <span class="tex-span"><i>m</i></span> distinct characters, print any of them.</p>





```input1
aaaaa
4

```




```input2
abacaba
4

```




```input3
abcdefgh
10

```




```output1
1
aaaaa

```




```output2
1
aaaa

```




```output3
0


```



## Note

<p>In the first sample the string consists of five identical letters but you are only allowed to delete 4 of them so that there was at least one letter left. Thus, the right answer is 1 and any string consisting of characters "<span class="tex-font-style-tt">a</span>" from 1 to 5 in length.</p><p>In the second sample you are allowed to delete 4 characters. You cannot delete all the characters, because the string has length equal to 7. However, you can delete all characters apart from "<span class="tex-font-style-tt">a</span>" (as they are no more than four), which will result in the "<span class="tex-font-style-tt">aaaa</span>" string.</p><p>In the third sample you are given a line whose length is equal to 8, and <span class="tex-span"><i>k</i> = 10</span>, so that the whole line can be deleted. The correct answer is 0 and an empty string.</p>
