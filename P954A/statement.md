## Description

<div><p>Mikhail walks on a 2D plane. He can go either up or right. You are given a sequence of Mikhail's moves. He thinks that this sequence is too long and he wants to make it as short as possible.</p><p>In the given sequence moving up is described by character <span class="tex-font-style-tt">U</span> and moving right is described by character <span class="tex-font-style-tt">R</span>. Mikhail can replace any pair of consecutive moves <span class="tex-font-style-tt">RU</span> or <span class="tex-font-style-tt">UR</span> with a diagonal move (described as character <span class="tex-font-style-tt">D</span>). After that, he can go on and do some other replacements, until there is no pair of consecutive moves <span class="tex-font-style-tt">RU</span> or <span class="tex-font-style-tt">UR</span> left.</p><p>Your problem is to print the minimum possible length of the sequence of moves after the replacements.</p></div><div class="input-specification"><p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the sequence. The second line contains the sequence consisting of <span class="tex-span"><i>n</i></span> characters <span class="tex-font-style-tt">U</span> and <span class="tex-font-style-tt">R</span>.</p></div><div class="output-specification"><p>Print the minimum possible length of the sequence of moves after all replacements are done.</p></div>

## Input

<p>The first line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— the length of the sequence. The second line contains the sequence consisting of <span class="tex-span"><i>n</i></span> characters <span class="tex-font-style-tt">U</span> and <span class="tex-font-style-tt">R</span>.</p>

## Output

<p>Print the minimum possible length of the sequence of moves after all replacements are done.</p>





```input1
5
RUURU

```




```input2
17
UUURRRRRUUURURUUU

```




```output1
3

```




```output2
13

```



## Note

<p>In the first test the shortened sequence of moves may be <span class="tex-font-style-tt">DUD</span> (its length is <span class="tex-span">3</span>).</p><p>In the second test the shortened sequence of moves can be <span class="tex-font-style-tt">UUDRRRDUDDUUU</span> (its length is <span class="tex-span">13</span>).</p>
