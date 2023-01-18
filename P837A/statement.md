## Description

<div><p>You are given a text of single-space separated words, consisting of small and capital Latin letters.</p><p><span class="tex-font-style-it">Volume</span> of the word is number of capital letters in the word. <span class="tex-font-style-it">Volume</span> of the text is maximum <span class="tex-font-style-it">volume</span> of all words in the text.</p><p>Calculate the <span class="tex-font-style-it">volume</span> of the given text.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — length of the text.</p><p>The second line contains text of single-space separated words <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>i</i></sub></span>, consisting only of small and capital Latin letters.</p></div><div class="output-specification"><p>Print one integer number — <span class="tex-font-style-it">volume</span> of text.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>) — length of the text.</p><p>The second line contains text of single-space separated words <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>i</i></sub></span>, consisting only of small and capital Latin letters.</p>

## Output

<p>Print one integer number — <span class="tex-font-style-it">volume</span> of text.</p>





```input1
7
NonZERO

```




```input2
24
this is zero answer text

```




```input3
24
Harbour Space University

```




```output1
5

```




```output2
0

```




```output3
1

```



## Note

<p>In the first example there is only one word, there are <span class="tex-font-style-tt">5</span> capital letters in it.</p><p>In the second example all of the words contain <span class="tex-font-style-tt">0</span> capital letters.</p>
