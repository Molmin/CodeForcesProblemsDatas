## Description

<div><p>Your friend recently gave you some slimes for your birthday. You have <span class="tex-span"><i>n</i></span> slimes all initially with value <span class="tex-span">1</span>.</p><p>You are going to play a game with these slimes. Initially, you put a single slime by itself in a row. Then, you will add the other <span class="tex-span"><i>n</i> - 1</span> slimes one by one. When you add a slime, you place it at the right of all already placed slimes. Then, while the last two slimes in the row have the same value <span class="tex-span"><i>v</i></span>, you combine them together to create a slime with value <span class="tex-span"><i>v</i> + 1</span>.</p><p>You would like to see what the final state of the row is after you've added all <span class="tex-span"><i>n</i></span> slimes. Please print the values of the slimes in the row from left to right.</p></div><div class="input-specification"><p>The first line of the input will contain a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>).</p></div><div class="output-specification"><p>Output a single line with <span class="tex-span"><i>k</i></span> integers, where <span class="tex-span"><i>k</i></span> is the number of slimes in the row after you've finished the procedure described in the problem statement. The <span class="tex-span"><i>i</i></span>-th of these numbers should be the value of the <span class="tex-span"><i>i</i></span>-th slime from the left.</p></div>

## Input

<p>The first line of the input will contain a single integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>).</p>

## Output

<p>Output a single line with <span class="tex-span"><i>k</i></span> integers, where <span class="tex-span"><i>k</i></span> is the number of slimes in the row after you've finished the procedure described in the problem statement. The <span class="tex-span"><i>i</i></span>-th of these numbers should be the value of the <span class="tex-span"><i>i</i></span>-th slime from the left.</p>





```input1
1

```




```input2
2

```




```input3
3

```




```input4
8

```




```output1
1

```




```output2
2

```




```output3
2 1

```




```output4
4

```



## Note

<p>In the first sample, we only have a single slime with value <span class="tex-span">1</span>. The final state of the board is just a single slime with value <span class="tex-span">1</span>.</p><p>In the second sample, we perform the following steps:</p><p>Initially we place a single slime in a row by itself. Thus, row is initially <span class="tex-font-style-tt">1</span>.</p><p>Then, we will add another slime. The row is now <span class="tex-font-style-tt">1 1</span>. Since two rightmost slimes have the same values, we should replace these slimes with one with value <span class="tex-span">2</span>. Thus, the final state of the board is <span class="tex-font-style-tt">2</span>.</p><p>In the third sample, after adding the first two slimes, our row is <span class="tex-font-style-tt">2</span>. After adding one more slime, the row becomes <span class="tex-font-style-tt">2 1</span>.</p><p>In the last sample, the steps look as follows: </p><ol> <li> <span class="tex-font-style-tt">1</span> </li><li> <span class="tex-font-style-tt">2</span> </li><li> <span class="tex-font-style-tt">2 1</span> </li><li> <span class="tex-font-style-tt">3</span> </li><li> <span class="tex-font-style-tt">3 1</span> </li><li> <span class="tex-font-style-tt">3 2</span> </li><li> <span class="tex-font-style-tt">3 2 1</span> </li><li> <span class="tex-font-style-tt">4</span> </li></ol>
