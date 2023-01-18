## Description

<div><p>Calvin the robot lies in an infinite rectangular grid. Calvin's source code contains a list of <span class="tex-span"><i>n</i></span> commands, each either '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>', or '<span class="tex-font-style-tt">L</span>'&nbsp;— instructions to move a single square up, right, down, or left, respectively. How many ways can Calvin execute a non-empty contiguous substrings of commands and return to the same square he starts in? Two substrings are considered different if they have different starting or ending indices.</p></div><div class="input-specification"><p>The first line of the input contains a single positive integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>)&nbsp;— the number of commands.</p><p>The next line contains <span class="tex-span"><i>n</i></span> characters, each either '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>', or '<span class="tex-font-style-tt">L</span>'&nbsp;— Calvin's source code.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of contiguous substrings that Calvin can execute and return to his starting square.</p></div>

## Input

<p>The first line of the input contains a single positive integer, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>)&nbsp;— the number of commands.</p><p>The next line contains <span class="tex-span"><i>n</i></span> characters, each either '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>', or '<span class="tex-font-style-tt">L</span>'&nbsp;— Calvin's source code.</p>

## Output

<p>Print a single integer&nbsp;— the number of contiguous substrings that Calvin can execute and return to his starting square.</p>





```input1
6
URLLDR

```




```input2
4
DLUU

```




```input3
7
RLRLRLR

```




```output1
2

```




```output2
0

```




```output3
12

```



## Note

<p>In the first case, the entire source code works, as well as the "<span class="tex-font-style-tt">RL</span>" substring in the second and third characters.</p><p>Note that, in the third case, the substring "<span class="tex-font-style-tt">LR</span>" appears three times, and is therefore counted three times to the total result.</p>
