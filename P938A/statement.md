## Description

<div><p>Victor tries to write his own text editor, with word correction included. However, the rules of word correction are really strange.</p><p>Victor thinks that if a word contains two <span class="tex-font-style-bf">consecutive</span> vowels, then it's kinda weird and it needs to be replaced. So the word corrector works in such a way: as long as there are two consecutive vowels in the word, it deletes the first vowel in a word such that there is <span class="tex-font-style-bf">another vowel right before it</span>. If there are no two consecutive vowels in the word, it is considered to be correct.</p><p>You are given a word <span class="tex-span"><i>s</i></span>. Can you predict what will it become after correction?</p><p><span class="tex-font-style-bf">In this problem letters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">e</span>, <span class="tex-font-style-tt">i</span>, <span class="tex-font-style-tt">o</span>, <span class="tex-font-style-tt">u</span> and <span class="tex-font-style-tt">y</span> are considered to be vowels</span>.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of letters in word <span class="tex-span"><i>s</i></span> before the correction.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> consisting of exactly <span class="tex-span"><i>n</i></span> lowercase Latin letters — the word before the correction.</p></div><div class="output-specification"><p>Output the word <span class="tex-span"><i>s</i></span> after the correction.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of letters in word <span class="tex-span"><i>s</i></span> before the correction.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> consisting of exactly <span class="tex-span"><i>n</i></span> lowercase Latin letters — the word before the correction.</p>

## Output

<p>Output the word <span class="tex-span"><i>s</i></span> after the correction.</p>





```input1
5
weird

```




```input2
4
word

```




```input3
5
aaeaa

```




```output1
werd

```




```output2
word

```




```output3
a

```



## Note

<p>Explanations of the examples:</p><ol> <li> There is only one replace: w<span class="tex-font-style-bf">ei</span>rd <img align="middle" class="tex-formula" src="file://HZQz2vOw.png" style="max-width: 100.0%;max-height: 100.0%;"> werd;</li><li> No replace needed since there are no two consecutive vowels;</li><li> <span class="tex-font-style-bf">aa</span>eaa <img align="middle" class="tex-formula" src="file://sBUyu2Z9.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-bf">ae</span>aa <img align="middle" class="tex-formula" src="file://tiuxYXjr.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-bf">aa</span>a <img align="middle" class="tex-formula" src="file://nozt7jxy.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-bf">aa</span> <img align="middle" class="tex-formula" src="file://nldDOABg.png" style="max-width: 100.0%;max-height: 100.0%;"> a. </li></ol>
