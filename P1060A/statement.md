## Description

<div><p>Let's call a string <span class="tex-font-style-it">a phone number</span> if it has length 11 and fits the pattern "<span class="tex-font-style-tt">8xxxxxxxxxx</span>", where each "<span class="tex-font-style-tt">x</span>" is replaced by a digit.</p><p>For example, "<span class="tex-font-style-tt">80123456789</span>" and "<span class="tex-font-style-tt">80000000000</span>" are phone numbers, while "<span class="tex-font-style-tt">8012345678</span>" and "<span class="tex-font-style-tt">79000000000</span>" are not.</p><p>You have $n$ cards with digits, and you want to use them to make as many phone numbers as possible. Each card must be used in at most one phone number, and you don't have to use all cards. The phone numbers do not necessarily have to be distinct.</p></div><div class="input-specification"><p>The first line contains an integer $n$&nbsp;— the number of cards with digits that you have ($1 \leq n \leq 100$).</p><p>The second line contains a string of $n$ digits (characters "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">1</span>", ..., "<span class="tex-font-style-tt">9</span>") $s_1, s_2, \ldots, s_n$. The string will not contain any other characters, such as leading or trailing spaces.</p></div><div class="output-specification"><p>If at least one phone number can be made from these cards, output the maximum number of phone numbers that can be made. Otherwise, output 0.</p></div>

## Input

<p>The first line contains an integer $n$&nbsp;— the number of cards with digits that you have ($1 \leq n \leq 100$).</p><p>The second line contains a string of $n$ digits (characters "<span class="tex-font-style-tt">0</span>", "<span class="tex-font-style-tt">1</span>", ..., "<span class="tex-font-style-tt">9</span>") $s_1, s_2, \ldots, s_n$. The string will not contain any other characters, such as leading or trailing spaces.</p>

## Output

<p>If at least one phone number can be made from these cards, output the maximum number of phone numbers that can be made. Otherwise, output 0.</p>





```input1
11
00000000008

```




```input2
22
0011223344556677889988

```




```input3
11
31415926535

```




```output1
1

```




```output2
2

```




```output3
0

```



## Note

<p>In the first example, one phone number, "<span class="tex-font-style-tt">8000000000</span>", can be made from these cards.</p><p>In the second example, you can make two phone numbers from the cards, for example, "<span class="tex-font-style-tt">80123456789</span>" and "<span class="tex-font-style-tt">80123456789</span>".</p><p>In the third example you can't make any phone number from the given cards.</p>
