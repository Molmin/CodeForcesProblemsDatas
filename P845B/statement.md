## Description

<div><p>Luba has a ticket consisting of <span class="tex-span">6</span> digits. In one move she can choose digit in any position and replace it with arbitrary digit. She wants to know the minimum number of digits she needs to replace in order to make the ticket lucky.</p><p>The ticket is considered lucky if the sum of first three digits equals to the sum of last three digits.</p></div><div class="input-specification"><p>You are given a string consisting of <span class="tex-span">6</span> characters (all characters are digits from <span class="tex-span">0</span> to <span class="tex-span">9</span>) — this string denotes Luba's ticket. The ticket can start with the digit <span class="tex-span">0</span>.</p></div><div class="output-specification"><p>Print one number — the minimum possible number of digits Luba needs to replace to make the ticket lucky.</p></div>

## Input

<p>You are given a string consisting of <span class="tex-span">6</span> characters (all characters are digits from <span class="tex-span">0</span> to <span class="tex-span">9</span>) — this string denotes Luba's ticket. The ticket can start with the digit <span class="tex-span">0</span>.</p>

## Output

<p>Print one number — the minimum possible number of digits Luba needs to replace to make the ticket lucky.</p>





```input1
000000

```




```input2
123456

```




```input3
111000

```




```output1
0

```




```output2
2

```




```output3
1

```



## Note

<p>In the first example the ticket is already lucky, so the answer is <span class="tex-span">0</span>.</p><p>In the second example Luba can replace <span class="tex-span">4</span> and <span class="tex-span">5</span> with zeroes, and the ticket will become lucky. It's easy to see that at least two replacements are required.</p><p>In the third example Luba can replace any zero with <span class="tex-span">3</span>. It's easy to see that at least one replacement is required.</p>
