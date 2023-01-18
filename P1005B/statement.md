## Description

<div><p>You are given two strings $s$ and $t$. In a single move, you can choose any of two strings and delete the first (that is, the leftmost) character. After a move, the length of the string decreases by $1$. You can't choose a string if it is empty.</p><p>For example:</p><ul> <li> by applying a move to the string "<span class="tex-font-style-tt">where</span>", the result is the string "<span class="tex-font-style-tt">here</span>", </li><li> by applying a move to the string "<span class="tex-font-style-tt">a</span>", the result is an empty string "". </li></ul><p>You are required to make two given strings equal using the fewest number of moves. It is possible that, in the end, both strings will be equal to the empty string, and so, are equal to each other. In this case, the answer is obviously the sum of the lengths of the initial strings.</p><p>Write a program that finds the minimum number of moves to make two given strings $s$ and $t$ equal.</p></div><div class="input-specification"><p>The first line of the input contains $s$. In the second line of the input contains $t$. Both strings consist only of lowercase Latin letters. The number of letters in each string is between 1 and $2\cdot10^5$, inclusive.</p></div><div class="output-specification"><p>Output the fewest number of moves required. It is possible that, in the end, both strings will be equal to the empty string, and so, are equal to each other. In this case, the answer is obviously the sum of the lengths of the given strings.</p></div>

## Input

<p>The first line of the input contains $s$. In the second line of the input contains $t$. Both strings consist only of lowercase Latin letters. The number of letters in each string is between 1 and $2\cdot10^5$, inclusive.</p>

## Output

<p>Output the fewest number of moves required. It is possible that, in the end, both strings will be equal to the empty string, and so, are equal to each other. In this case, the answer is obviously the sum of the lengths of the given strings.</p>





```input1
test
west

```




```input2
codeforces
yes

```




```input3
test
yes

```




```input4
b
ab

```




```output1
2

```




```output2
9

```




```output3
7

```




```output4
1

```



## Note

<p>In the first example, you should apply the move once to the first string and apply the move once to the second string. As a result, both strings will be equal to "<span class="tex-font-style-tt">est</span>".</p><p>In the second example, the move should be applied to the string "<span class="tex-font-style-tt">codeforces</span>" $8$ times. As a result, the string becomes "<span class="tex-font-style-tt"><span class="tex-font-style-striked">codeforc</span>es</span>" $\to$ "<span class="tex-font-style-tt">es</span>". The move should be applied to the string "<span class="tex-font-style-tt">yes</span>" once. The result is the same string "<span class="tex-font-style-tt"><span class="tex-font-style-striked">y</span>es</span>" $\to$ "<span class="tex-font-style-tt">es</span>".</p><p>In the third example, you can make the strings equal only by completely deleting them. That is, in the end, both strings will be empty.</p><p>In the fourth example, the first character of the second string should be deleted.</p>
