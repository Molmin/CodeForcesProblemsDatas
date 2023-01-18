## Description

<div><p>You all know that the Library of Bookland is the largest library in the world. There are dozens of thousands of books in the library.</p><p><span class="tex-font-style-it">Some long and uninteresting story was removed...</span></p><p>The alphabet of Bookland is so large that its letters are denoted by positive integers. Each letter can be small or large, the large version of a letter <span class="tex-span"><i>x</i></span> is denoted by <span class="tex-span"><i>x</i>'</span>. BSCII encoding, which is used everywhere in Bookland, is made in that way so that large letters are presented in the order of the numbers they are denoted by, and small letters are presented in the order of the numbers they are denoted by, but all large letters are <span class="tex-font-style-bf">before</span> all small letters. For example, the following conditions hold: <span class="tex-span">2 &lt; 3</span>, <span class="tex-span">2' &lt; 3'</span>, <span class="tex-span">3' &lt; 2</span>.</p><p>A word <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>a</i></sub></span> is not <span class="tex-font-style-it">lexicographically</span> greater than <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>b</i></sub></span> if one of the two following conditions holds: </p><ul> <li> <span class="tex-span"><i>a</i> ≤ <i>b</i></span> and <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>a</i></sub> = <i>y</i><sub class="lower-index"><i>a</i></sub></span>, i.e. the first word is the prefix of the second word; </li><li> there is a position <span class="tex-span">1 ≤ <i>j</i> ≤ <i>min</i>(<i>a</i>, <i>b</i>)</span>, such that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, ..., <i>x</i><sub class="lower-index"><i>j</i> - 1</sub> = <i>y</i><sub class="lower-index"><i>j</i> - 1</sub></span> and <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> &lt; <i>y</i><sub class="lower-index"><i>j</i></sub></span>, i.e. at the first position where the words differ the first word has a smaller letter than the second word has. </li></ul> <p>For example, the word "<span class="tex-span">3'</span> <span class="tex-span">7</span> <span class="tex-span">5</span>" is before the word "<span class="tex-span">2</span> <span class="tex-span">4'</span> <span class="tex-span">6</span>" in lexicographical order. It is said that sequence of words is in lexicographical order if each word is not lexicographically greater than the next word in the sequence.</p><p>Denis has a sequence of words consisting of small letters only. He wants to change some letters to large (let's call this process a <span class="tex-font-style-it">capitalization</span>) in such a way that the sequence of words is in lexicographical order. However, he soon realized that for some reason he can't change a single letter in a single word. He only can choose a letter and change all of its occurrences in <span class="tex-font-style-bf">all</span> words to large letters. He can perform this operation any number of times with arbitrary letters of Bookland's alphabet.</p><p>Help Denis to choose which letters he needs to capitalize (make large) in order to make the sequence of words lexicographically ordered, or determine that it is impossible.</p><p>Note that some words can be <span class="tex-font-style-bf">equal</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of words and the number of letters in Bookland's alphabet, respectively. The letters of Bookland's alphabet are denoted by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a description of one word in format <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>s</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>s</i><sub class="lower-index"><i>i</i>, <i>l</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>m</i></span>), where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is the length of the word, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is the sequence of letters in the word. The words are given in the order Denis has them in the sequence.</p><p>It is guaranteed that the total length of all words is not greater than <span class="tex-span">100 000</span>.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">Yes</span>" (without quotes), if it is possible to capitalize some set of letters in such a way that the sequence of words becomes lexicographically ordered. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without quotes).</p><p>If the required is possible, in the second line print <span class="tex-span"><i>k</i></span>&nbsp;— the number of letters Denis has to capitalize (make large), and in the third line print <span class="tex-span"><i>k</i></span> distinct integers&nbsp;— these letters. Note that you <span class="tex-font-style-bf">don't need to minimize</span> the value <span class="tex-span"><i>k</i></span>.</p><p>You can print the letters in any order. If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>)&nbsp;— the number of words and the number of letters in Bookland's alphabet, respectively. The letters of Bookland's alphabet are denoted by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains a description of one word in format <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>s</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>s</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>s</i><sub class="lower-index"><i>i</i>, <i>l</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>m</i></span>), where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is the length of the word, and <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is the sequence of letters in the word. The words are given in the order Denis has them in the sequence.</p><p>It is guaranteed that the total length of all words is not greater than <span class="tex-span">100 000</span>.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">Yes</span>" (without quotes), if it is possible to capitalize some set of letters in such a way that the sequence of words becomes lexicographically ordered. Otherwise, print "<span class="tex-font-style-tt">No</span>" (without quotes).</p><p>If the required is possible, in the second line print <span class="tex-span"><i>k</i></span>&nbsp;— the number of letters Denis has to capitalize (make large), and in the third line print <span class="tex-span"><i>k</i></span> distinct integers&nbsp;— these letters. Note that you <span class="tex-font-style-bf">don't need to minimize</span> the value <span class="tex-span"><i>k</i></span>.</p><p>You can print the letters in any order. If there are multiple answers, print any of them.</p>





```input1
4 3
1 2
1 1
3 1 3 2
2 1 1

```




```input2
6 5
2 1 2
2 1 2
3 1 2 3
2 1 5
2 4 4
2 4 4

```




```input3
4 3
4 3 2 2 1
3 1 1 3
3 2 3 3
2 3 1

```




```output1
Yes
2
2 3
```




```output2
Yes
0

```




```output3
No

```



## Note

<p>In the first example after Denis makes letters <span class="tex-span">2</span> and <span class="tex-span">3</span> large, the sequence looks like the following:</p><ul> <li> <span class="tex-span">2'</span> </li><li> <span class="tex-span">1</span> </li><li> <span class="tex-span">1</span> <span class="tex-span">3'</span> <span class="tex-span">2'</span> </li><li> <span class="tex-span">1</span> <span class="tex-span">1</span> </li></ul><p>The condition <span class="tex-span">2' &lt; 1</span> holds, so the first word is not lexicographically larger than the second word. The second word is the prefix of the third word, so the are in lexicographical order. As the first letters of the third and the fourth words are the same, and <span class="tex-span">3' &lt; 1</span>, then the third word is not lexicographically larger than the fourth word.</p><p>In the second example the words are in lexicographical order from the beginning, so Denis can do nothing.</p><p>In the third example there is no set of letters such that if Denis capitalizes them, the sequence becomes lexicographically ordered.</p>
