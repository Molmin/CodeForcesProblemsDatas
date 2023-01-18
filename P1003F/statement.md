## Description

<div><p>You are given a text consisting of $n$ space-separated words. There is exactly one space character between any pair of adjacent words. There are no spaces before the first word and no spaces after the last word. The length of text is the number of letters and spaces in it. $w_i$ is the $i$-th word of text. All words consist only of lowercase Latin letters.</p><p>Let's denote a segment of words $w[i..j]$ as a sequence of words $w_i, w_{i + 1}, \dots, w_j$. Two segments of words $w[i_1 .. j_1]$ and $w[i_2 .. j_2]$ are considered <span class="tex-font-style-bf">equal</span> if $j_1 - i_1 = j_2 - i_2$, $j_1 \ge i_1$, $j_2 \ge i_2$, and for every $t \in [0, j_1 - i_1]$ $w_{i_1 + t} = w_{i_2 + t}$. For example, for the text "<span class="tex-font-style-tt">to be or not to be</span>" the segments $w[1..2]$ and $w[5..6]$ are equal, they correspond to the words "<span class="tex-font-style-tt">to be</span>".</p><p>An abbreviation is a replacement of some segments of words with their first <span class="tex-font-style-bf">uppercase</span> letters. In order to perform an abbreviation, you have to choose <span class="tex-font-style-bf">at least two</span> non-intersecting equal segments of words, and replace each chosen segment with the string consisting of first letters of the words in the segment (written in uppercase). For example, for the text "<span class="tex-font-style-tt">a ab a a b ab a a b c</span>" you can replace segments of words $w[2..4]$ and $w[6..8]$ with an abbreviation "<span class="tex-font-style-tt">AAA</span>" and obtain the text "<span class="tex-font-style-tt">a AAA b AAA b c</span>", or you can replace segments of words $w[2..5]$ and $w[6..9]$ with an abbreviation "<span class="tex-font-style-tt">AAAB</span>" and obtain the text "<span class="tex-font-style-tt">a AAAB AAAB c</span>".</p><p>What is the minimum length of the text after at most one abbreviation?</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1 \le n \le 300$) — the number of words in the text.</p><p>The next line contains $n$ space-separated words of the text $w_1, w_2, \dots, w_n$. Each word consists only of lowercase Latin letters.</p><p>It is guaranteed that the length of text does not exceed $10^5$.</p></div><div class="output-specification"><p>Print one integer — the minimum length of the text after at most one abbreviation.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1 \le n \le 300$) — the number of words in the text.</p><p>The next line contains $n$ space-separated words of the text $w_1, w_2, \dots, w_n$. Each word consists only of lowercase Latin letters.</p><p>It is guaranteed that the length of text does not exceed $10^5$.</p>

## Output

<p>Print one integer — the minimum length of the text after at most one abbreviation.</p>





```input1
6
to be or not to be

```




```input2
10
a ab a a b ab a a b c

```




```input3
6
aa bb aa aa bb bb

```




```output1
12

```




```output2
13

```




```output3
11

```



## Note

<p>In the first example you can obtain the text "<span class="tex-font-style-tt">TB or not TB</span>".</p><p>In the second example you can obtain the text "<span class="tex-font-style-tt">a AAAB AAAB c</span>".</p><p>In the third example you can obtain the text "<span class="tex-font-style-tt">AB aa AB bb</span>".</p>
