## Description

<div><p>One of the Hedgehog and his friend's favorite entertainments is to take some sentence or a song and replace half of the words (sometimes even all of them) with each other's names.</p><p>The friend's birthday is approaching and the Hedgehog decided to make a special present to his friend: a very long song, where his name will be repeated many times. But try as he might, he can't write a decent song!</p><p>The problem is that the Hedgehog has already decided how long the resulting sentence should be (i.e. how many letters it should contain) and in which positions in the sentence the friend's name should occur, and it must not occur in any other position in the sentence. Besides, the Hedgehog decided to limit himself to using only the first <span class="tex-span"><i>K</i></span> letters of an English alphabet in this sentence (so it will be not even a sentence, but one long word).</p><p>The resulting problem is indeed quite complicated, that's why the Hedgehog asks you to help him and write a program that will make the desired word by the given name <span class="tex-span"><i>P</i></span>, the length <span class="tex-span"><i>N</i></span> of the required word, the given positions of the occurrences of the name <span class="tex-span"><i>P</i></span> in the desired word and the alphabet's size <span class="tex-span"><i>K</i></span>. Note that the occurrences of the name can overlap with each other.</p></div><div class="input-specification"><p>The first line contains numbers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> which are the length of the required string and the alphabet size accordingly. The limitations are: <span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>K</i> ≤ 26</span>.</p><p>The second line contains the name <span class="tex-span"><i>P</i></span> which is a non-empty string whose length does not exceed <span class="tex-span"><i>N</i></span> characters. The string consists only of the first <span class="tex-span"><i>K</i></span> lowercase symbols of an English alphabet.</p><p>The third line contains the string of length <span class="tex-span"><i>N</i> - <i>length</i>(<i>P</i>) + 1</span>, consisting only of numbers zero and one. A number one in the <span class="tex-span"><i>i</i></span>-th position means that an occurrence of the name <span class="tex-span"><i>P</i></span> should start from <span class="tex-span"><i>i</i></span>-th position of the desired word, while a zero means that there is no occurrence starting here. </p></div><div class="output-specification"><p>Print the desired word <span class="tex-span"><i>S</i></span>. If there are several answers, print any of them.</p><p>If there is no solution, then print "No solution".</p></div>

## Input

<p>The first line contains numbers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i></span> which are the length of the required string and the alphabet size accordingly. The limitations are: <span class="tex-span">1 ≤ <i>N</i> ≤ 100</span>, <span class="tex-span">2 ≤ <i>K</i> ≤ 26</span>.</p><p>The second line contains the name <span class="tex-span"><i>P</i></span> which is a non-empty string whose length does not exceed <span class="tex-span"><i>N</i></span> characters. The string consists only of the first <span class="tex-span"><i>K</i></span> lowercase symbols of an English alphabet.</p><p>The third line contains the string of length <span class="tex-span"><i>N</i> - <i>length</i>(<i>P</i>) + 1</span>, consisting only of numbers zero and one. A number one in the <span class="tex-span"><i>i</i></span>-th position means that an occurrence of the name <span class="tex-span"><i>P</i></span> should start from <span class="tex-span"><i>i</i></span>-th position of the desired word, while a zero means that there is no occurrence starting here. </p>

## Output

<p>Print the desired word <span class="tex-span"><i>S</i></span>. If there are several answers, print any of them.</p><p>If there is no solution, then print "No solution".</p>





```input1
5 2
aba
101

```




```input2
5 2
a
10001

```




```input3
6 2
abba
101

```




```output1
ababa
```




```output2
abbba
```




```output3
No solution
```


