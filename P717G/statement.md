## Description

<div><p>You have recently fallen through a hole and, after several hours of unconsciousness, have realized you are in an underground city. On one of your regular, daily walks through the unknown, you have encountered two unusually looking skeletons called Sanz and P’pairus, who decided to accompany you and give you some puzzles for seemingly unknown reasons.</p><p>One day, Sanz has created a crossword for you. Not any kind of crossword, but a 1D crossword! You are given <span class="tex-span"><i>m</i></span> words and a string of length <span class="tex-span"><i>n</i></span>. You are also given an array <span class="tex-span"><i>p</i></span>, which designates how much each word is worth&nbsp;— the <span class="tex-span"><i>i</i></span>-th word is worth <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> points. Whenever you find one of the <span class="tex-span"><i>m</i></span> words in the string, you are given the corresponding number of points. Each position in the crossword can be used at most <span class="tex-span"><i>x</i></span> times. A certain word can be counted at different places, but you cannot count the same appearance of a word multiple times. If a word is a substring of another word, you can count them both (presuming you haven’t used the positions more than <span class="tex-span"><i>x</i></span> times).</p><p>In order to solve the puzzle, you need to tell Sanz what’s the maximum achievable number of points in the crossword. There is no need to cover all postions, just get the maximal score! Crossword and words contain only lowercase English letters.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the length of the crossword. The second line contains the crossword string. The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of given words, and next <span class="tex-span"><i>m</i></span> lines contain description of words: each line will have a string representing a non-empty word (its length doesn't exceed the length of the crossword) and integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). Last line of the input will contain <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 100</span>)&nbsp;— maximum number of times a position in crossword can be used.</p></div><div class="output-specification"><p>Output single integer&nbsp;— maximum number of points you can get.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>)&nbsp;— the length of the crossword. The second line contains the crossword string. The third line contains a single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>)&nbsp;— the number of given words, and next <span class="tex-span"><i>m</i></span> lines contain description of words: each line will have a string representing a non-empty word (its length doesn't exceed the length of the crossword) and integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>). Last line of the input will contain <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 100</span>)&nbsp;— maximum number of times a position in crossword can be used.</p>

## Output

<p>Output single integer&nbsp;— maximum number of points you can get.</p>





```input1
6
abacba
2
aba 6
ba 3
3

```




```output1
12

```



## Note

<p>For example, with the string "<span class="tex-font-style-tt">abacba</span>", words "<span class="tex-font-style-tt">aba</span>" (6 points) and "<span class="tex-font-style-tt">ba</span>" (3 points), and <span class="tex-span"><i>x</i> = 3</span>, you can get at most <span class="tex-span">12</span> points - the word "<span class="tex-font-style-tt">aba</span>" appears once ("<span class="tex-font-style-tt">abacba</span>"), while "<span class="tex-font-style-tt">ba</span>" appears two times ("<span class="tex-font-style-tt">abacba</span>"). Note that for <span class="tex-span"><i>x</i> = 1</span>, you could get at most <span class="tex-span">9</span> points, since you wouldn’t be able to count both "<span class="tex-font-style-tt">aba</span>" and the first appearance of "<span class="tex-font-style-tt">ba</span>".</p>
