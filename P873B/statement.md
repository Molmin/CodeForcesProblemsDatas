## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span> consisting only of characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. A substring <span class="tex-span">[<i>l</i>, <i>r</i>]</span> of <span class="tex-span"><i>s</i></span> is a string <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub><i>s</i><sub class="lower-index"><i>l</i> + 2</sub>... <i>s</i><sub class="lower-index"><i>r</i></sub></span>, and its length equals to <span class="tex-span"><i>r</i> - <i>l</i> + 1</span>. A substring is called <span class="tex-font-style-it">balanced</span> if the number of zeroes (<span class="tex-font-style-tt">0</span>) equals to the number of ones in this substring.</p><p>You have to determine the length of the longest <span class="tex-font-style-it">balanced</span> substring of <span class="tex-span"><i>s</i></span>.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of characters in <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> consisting of exactly <span class="tex-span"><i>n</i></span> characters. Only characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> can appear in <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>If there is no non-empty <span class="tex-font-style-it">balanced</span> substring in <span class="tex-span"><i>s</i></span>, print <span class="tex-font-style-tt">0</span>. Otherwise, print the length of the longest <span class="tex-font-style-it">balanced</span> substring.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100000</span>) — the number of characters in <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> consisting of exactly <span class="tex-span"><i>n</i></span> characters. Only characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span> can appear in <span class="tex-span"><i>s</i></span>.</p>

## Output

<p>If there is no non-empty <span class="tex-font-style-it">balanced</span> substring in <span class="tex-span"><i>s</i></span>, print <span class="tex-font-style-tt">0</span>. Otherwise, print the length of the longest <span class="tex-font-style-it">balanced</span> substring.</p>





```input1
8
11010111

```




```input2
3
111

```




```output1
4

```




```output2
0

```



## Note

<p>In the first example you can choose the substring <span class="tex-span">[3, 6]</span>. It is <span class="tex-font-style-it">balanced</span>, and its length is <span class="tex-span">4</span>. Choosing the substring <span class="tex-span">[2, 5]</span> is also possible.</p><p>In the second example it's impossible to find a non-empty <span class="tex-font-style-it">balanced</span> substring.</p>
