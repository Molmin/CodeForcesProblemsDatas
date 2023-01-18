## Description

<div><p>Beroffice text editor has a wide range of features that help working with text. One of the features is an automatic search for typos and suggestions of how to fix them.</p><p>Beroffice works only with small English letters (i.e. with 26 letters from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">z</span>). Beroffice thinks that a word is typed with a typo if there are three or more consonants in a row in the word. The only exception is that if the block of consonants has all letters the same, then this block (even if its length is greater than three) is not considered a typo. Formally, a word is typed with a typo if there is a block of not less that three consonants in a row, and there are at least two different letters in this block.</p><p>For example:</p><ul> <li> the following words have typos: "<span class="tex-font-style-tt">hellno</span>", "<span class="tex-font-style-tt">hackcerrs</span>" and "<span class="tex-font-style-tt">backtothefutttture</span>"; </li><li> the following words don't have typos: "<span class="tex-font-style-tt">helllllooooo</span>", "<span class="tex-font-style-tt">tobeornottobe</span>" and "<span class="tex-font-style-tt">oooooo</span>". </li></ul><p>When Beroffice editor finds a word with a typo, it inserts as little as possible number of spaces in this word (dividing it into several words) in such a way that each of the resulting words is typed without any typos.</p><p>Implement this feature of Beroffice editor. Consider the following letters as the only vowels: '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">i</span>', '<span class="tex-font-style-tt">o</span>' and '<span class="tex-font-style-tt">u</span>'. All the other letters are consonants in this problem.</p></div><div class="input-specification"><p>The only line contains a non-empty word consisting of small English letters. The length of the word is between <span class="tex-span">1</span> and <span class="tex-span">3000</span> letters.</p></div><div class="output-specification"><p>Print the given word without any changes if there are no typos.</p><p>If there is at least one typo in the word, insert the minimum number of spaces into the word so that each of the resulting words doesn't have any typos. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The only line contains a non-empty word consisting of small English letters. The length of the word is between <span class="tex-span">1</span> and <span class="tex-span">3000</span> letters.</p>

## Output

<p>Print the given word without any changes if there are no typos.</p><p>If there is at least one typo in the word, insert the minimum number of spaces into the word so that each of the resulting words doesn't have any typos. If there are multiple solutions, print any of them.</p>





```input1
hellno

```




```input2
abacaba

```




```input3
asdfasdf

```




```output1
hell no 

```




```output2
abacaba 

```




```output3
asd fasd f 

```


