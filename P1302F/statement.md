## Description

<div><p><span class="tex-font-style-it">This is an unusual problem in an unusual contest, here is the announcement: <a href="//codeforces.com/blog/entry/73543">http://codeforces.com/blog/entry/73543</a></span></p><p>You have the safe lock which consists of 5 decimal digits. If you rotate some digit, it increases by one, except 9 which becomes 0.</p><p>Initially, the lock contains number $x$. To unlock the safe you must do the following operations in order (and be careful, don't mix up if and else statements).</p><p>If sum of digits on positions 1 and 4 is greater than 10, rotate digit on position 1 by 3 times, else rotate digit on position 4 by 8 times.</p><p>If sum of digits on positions 3 and 2 is greater than 8, rotate digit on position 4 by 9 times, else rotate digit on position 5 by 8 times.</p><p>If digit on position 3 is odd, rotate digit on position 3 by 3 times, else rotate digit on position 3 by 4 times.</p><p>If digit on position 5 is greater than digit on position 2, rotate digit on position 4 by 1 times, else rotate digit on position 2 by 7 times.</p><p>If digit on position 1 is odd, rotate digit on position 1 by 3 times, else rotate digit on position 3 by 5 times.</p><p>If digit on position 4 is odd, rotate digit on position 4 by 7 times, else rotate digit on position 1 by 9 times.</p><p>If digit on position 4 is greater than digit on position 1, rotate digit on position 4 by 9 times, else rotate digit on position 4 by 2 times.</p><p>If digit on position 1 is greater than digit on position 3, rotate digit on position 2 by 1 times, else rotate digit on position 3 by 1 times.</p><p>If digit on position 5 is greater than digit on position 3, rotate digit on position 4 by 5 times, else rotate digit on position 5 by 8 times.</p><p>If sum of digits on positions 1 and 3 is greater than 8, rotate digit on position 4 by 5 times, else rotate digit on position 2 by 5 times.</p><p>If digit on position 1 is greater than digit on position 4, rotate digit on position 4 by 3 times, else rotate digit on position 2 by 3 times.</p><p>If sum of digits on positions 3 and 1 is greater than 9, rotate digit on position 2 by 9 times, else rotate digit on position 2 by 2 times.</p><p>If sum of digits on positions 4 and 3 is greater than 10, rotate digit on position 4 by 7 times, else rotate digit on position 5 by 7 times.</p><p>If digit on position 3 is greater than digit on position 2, rotate digit on position 3 by 2 times, else rotate digit on position 4 by 6 times.</p><p>If digit on position 1 is greater than digit on position 3, rotate digit on position 1 by 9 times, else rotate digit on position 2 by 9 times.</p><p>If digit on position 3 is odd, rotate digit on position 3 by 9 times, else rotate digit on position 1 by 5 times.</p><p>If sum of digits on positions 3 and 5 is greater than 9, rotate digit on position 3 by 4 times, else rotate digit on position 3 by 9 times.</p><p>If digit on position 3 is greater than digit on position 1, rotate digit on position 5 by 1 times, else rotate digit on position 5 by 7 times.</p><p>If digit on position 1 is greater than digit on position 3, rotate digit on position 2 by 9 times, else rotate digit on position 4 by 6 times.</p><p>If sum of digits on positions 2 and 3 is greater than 10, rotate digit on position 2 by 2 times, else rotate digit on position 3 by 6 times.</p></div><div class="input-specification"><p>Input contains single number $x$ consisting of exactly 5 digits, leading zeroes are allowed.</p></div><div class="output-specification"><p>Output the number after applying all operations.</p></div>

## Input

<p>Input contains single number $x$ consisting of exactly 5 digits, leading zeroes are allowed.</p>

## Output

<p>Output the number after applying all operations.</p>





```input1
00000
```




```input2
12345
```




```output1
61376
```




```output2
07769
```


