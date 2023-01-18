## Description

<div><p>You've got string <span class="tex-span"><i>s</i></span>, consisting of small English letters. Some of the English letters are <span class="tex-font-style-it">good</span>, the rest are <span class="tex-font-style-it">bad</span>.</p><p>A substring <span class="tex-span"><i>s</i>[<i>l</i>...<i>r</i>]</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>s</i>|</span>) of string <span class="tex-span"><i>s</i>  =  <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>...<i>s</i><sub class="lower-index">|<i>s</i>|</sub></span> (where <span class="tex-span">|<i>s</i>|</span> is the length of string <span class="tex-span"><i>s</i></span>) is string <span class="tex-span"> <i>s</i><sub class="lower-index"><i>l</i></sub><i>s</i><sub class="lower-index"><i>l</i> + 1</sub>...<i>s</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>The substring <span class="tex-span"><i>s</i>[<i>l</i>...<i>r</i>]</span> is <span class="tex-font-style-it">good</span>, if among the letters <span class="tex-span"> <i>s</i><sub class="lower-index"><i>l</i></sub>, <i>s</i><sub class="lower-index"><i>l</i> + 1</sub>, ..., <i>s</i><sub class="lower-index"><i>r</i></sub></span> there are <span class="tex-font-style-bf">at most</span> <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">bad</span> ones (look at the sample's explanation to understand it more clear).</p><p>Your task is to find the number of distinct good substrings of the given string <span class="tex-span"><i>s</i></span>. Two substrings <span class="tex-span"><i>s</i>[<i>x</i>...<i>y</i>]</span> and <span class="tex-span"><i>s</i>[<i>p</i>...<i>q</i>]</span> are considered distinct if their content is different, i.e. <span class="tex-span"><i>s</i>[<i>x</i>...<i>y</i>] ≠ <i>s</i>[<i>p</i>...<i>q</i>]</span>.</p></div><div class="input-specification"><p>The first line of the input is the non-empty string <span class="tex-span"><i>s</i></span>, consisting of small English letters, the string's length is at most <span class="tex-span">1500</span> characters.</p><p>The second line of the input is the string of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>", the length is exactly 26 characters. If the <span class="tex-span"><i>i</i></span>-th character of this string equals "<span class="tex-font-style-tt">1</span>", then the <span class="tex-span"><i>i</i></span>-th English letter is good, otherwise it's bad. That is, the first character of this string corresponds to letter "<span class="tex-font-style-tt">a</span>", the second one corresponds to letter "<span class="tex-font-style-tt">b</span>" and so on.</p><p>The third line of the input consists a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ |<i>s</i>|</span>) — the maximum acceptable number of bad characters in a good substring.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct good substrings of string <span class="tex-span"><i>s</i></span>.</p></div>

## Input

<p>The first line of the input is the non-empty string <span class="tex-span"><i>s</i></span>, consisting of small English letters, the string's length is at most <span class="tex-span">1500</span> characters.</p><p>The second line of the input is the string of characters "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">1</span>", the length is exactly 26 characters. If the <span class="tex-span"><i>i</i></span>-th character of this string equals "<span class="tex-font-style-tt">1</span>", then the <span class="tex-span"><i>i</i></span>-th English letter is good, otherwise it's bad. That is, the first character of this string corresponds to letter "<span class="tex-font-style-tt">a</span>", the second one corresponds to letter "<span class="tex-font-style-tt">b</span>" and so on.</p><p>The third line of the input consists a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ |<i>s</i>|</span>) — the maximum acceptable number of bad characters in a good substring.</p>

## Output

<p>Print a single integer — the number of distinct good substrings of string <span class="tex-span"><i>s</i></span>.</p>





```input1
ababab
01000000000000000000000000
1

```




```input2
acbacbacaa
00000000000000000000000000
2

```




```output1
5

```




```output2
8

```



## Note

<p>In the first example there are following good substrings: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">bab</span>".</p><p>In the second example there are following good substrings: "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ac</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">ca</span>", "<span class="tex-font-style-tt">cb</span>".</p>
