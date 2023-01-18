## Description

<div><p>Hurricane came to Berland and to suburbs Stringsvill. You are going to it to check if it's all right with you favorite string. Hurrinace broke it a bit by reversing some of its non-intersecting substrings. You have a photo of this string before hurricane and you want to restore it to original state using reversing minimum possible number of its substrings and find out which substrings you should reverse.</p><p>You are given a string <span class="tex-span"><i>s</i></span>&nbsp;— original state of your string and string <span class="tex-span"><i>t</i></span>&nbsp;— state of the string after hurricane. You should select <span class="tex-span"><i>k</i></span> non-intersecting substrings of <span class="tex-span"><i>t</i></span> in such a way that after reverse of these substrings string will be equal <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>k</i></span> is minimum possible.</p></div><div class="input-specification"><p>First line of input contains string <span class="tex-span"><i>s</i></span> and second line contains string <span class="tex-span"><i>t</i></span>. Both strings have same length and consist of lowercase English letters. <span class="tex-span">1 ≤ |<i>s</i>| = |<i>t</i>| ≤ 5·10<sup class="upper-index">5</sup></span></p></div><div class="output-specification"><p>In first line print <span class="tex-span"><i>k</i></span>&nbsp;— minimum number of substrings you should reverse. Next output <span class="tex-span"><i>k</i></span> lines. Each line should contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> meaning that you should reverse substring from symbol number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to symbol <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (strings are 1-indexed). These substrings shouldn't intersect. If there are multiple answers print any. If it's impossible to restore string output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>First line of input contains string <span class="tex-span"><i>s</i></span> and second line contains string <span class="tex-span"><i>t</i></span>. Both strings have same length and consist of lowercase English letters. <span class="tex-span">1 ≤ |<i>s</i>| = |<i>t</i>| ≤ 5·10<sup class="upper-index">5</sup></span></p>

## Output

<p>In first line print <span class="tex-span"><i>k</i></span>&nbsp;— minimum number of substrings you should reverse. Next output <span class="tex-span"><i>k</i></span> lines. Each line should contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> meaning that you should reverse substring from symbol number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to symbol <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (strings are 1-indexed). These substrings shouldn't intersect. If there are multiple answers print any. If it's impossible to restore string output <span class="tex-font-style-tt">-1</span>.</p>





```input1
abcxxxdef
cbaxxxfed

```




```output1
2
7 9
1 3

```


