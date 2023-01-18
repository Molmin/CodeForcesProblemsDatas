## Description

<div><p>Valentin participates in a show called "Shockers". The rules are quite easy: jury selects one letter which Valentin doesn't know. He should make a small speech, but every time he pronounces a word that contains the selected letter, he receives an electric shock. He can make guesses which letter is selected, but for each incorrect guess he receives an electric shock too. The show ends when Valentin guesses the selected letter correctly.</p><p>Valentin can't keep in mind everything, so he could guess the selected letter much later than it can be uniquely determined and get excessive electric shocks. Excessive electric shocks are those which Valentin got after the moment the selected letter can be uniquely determined. You should find out the number of excessive electric shocks.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of actions Valentin did.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain descriptions of his actions, each line contains description of one action. Each action can be of one of three types: </p><ol> <li> Valentin pronounced some word and didn't get an electric shock. This action is described by the string "<span class="tex-font-style-tt">. w</span>" (without quotes), in which "<span class="tex-font-style-tt">.</span>" is a dot (ASCII-code 46), and <span class="tex-span"><i>w</i></span> is the word that Valentin said. </li><li> Valentin pronounced some word and got an electric shock. This action is described by the string "<span class="tex-font-style-tt">! w</span>" (without quotes), in which "<span class="tex-font-style-tt">!</span>" is an exclamation mark (ASCII-code 33), and <span class="tex-span"><i>w</i></span> is the word that Valentin said. </li><li> Valentin made a guess about the selected letter. This action is described by the string "<span class="tex-font-style-tt">? s</span>" (without quotes), in which "<span class="tex-font-style-tt">?</span>" is a question mark (ASCII-code 63), and <span class="tex-span"><i>s</i></span> is the guess&nbsp;— a lowercase English letter. </li></ol><p>All words consist only of lowercase English letters. The total length of all words does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that last action is a guess about the selected letter. Also, it is guaranteed that Valentin didn't make correct guesses about the selected letter before the last action. Moreover, it's guaranteed that if Valentin got an electric shock after pronouncing some word, then it contains the selected letter; and also if Valentin didn't get an electric shock after pronouncing some word, then it does not contain the selected letter.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of electric shocks that Valentin could have avoided if he had told the selected letter just after it became uniquely determined.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of actions Valentin did.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain descriptions of his actions, each line contains description of one action. Each action can be of one of three types: </p><ol> <li> Valentin pronounced some word and didn't get an electric shock. This action is described by the string "<span class="tex-font-style-tt">. w</span>" (without quotes), in which "<span class="tex-font-style-tt">.</span>" is a dot (ASCII-code 46), and <span class="tex-span"><i>w</i></span> is the word that Valentin said. </li><li> Valentin pronounced some word and got an electric shock. This action is described by the string "<span class="tex-font-style-tt">! w</span>" (without quotes), in which "<span class="tex-font-style-tt">!</span>" is an exclamation mark (ASCII-code 33), and <span class="tex-span"><i>w</i></span> is the word that Valentin said. </li><li> Valentin made a guess about the selected letter. This action is described by the string "<span class="tex-font-style-tt">? s</span>" (without quotes), in which "<span class="tex-font-style-tt">?</span>" is a question mark (ASCII-code 63), and <span class="tex-span"><i>s</i></span> is the guess&nbsp;— a lowercase English letter. </li></ol><p>All words consist only of lowercase English letters. The total length of all words does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p>It is guaranteed that last action is a guess about the selected letter. Also, it is guaranteed that Valentin didn't make correct guesses about the selected letter before the last action. Moreover, it's guaranteed that if Valentin got an electric shock after pronouncing some word, then it contains the selected letter; and also if Valentin didn't get an electric shock after pronouncing some word, then it does not contain the selected letter.</p>

## Output

<p>Output a single integer&nbsp;— the number of electric shocks that Valentin could have avoided if he had told the selected letter just after it became uniquely determined.</p>





```input1
5
! abc
. ad
. b
! cd
? c

```




```input2
8
! hello
! codeforces
? c
. o
? d
? h
. l
? e

```




```input3
7
! ababahalamaha
? a
? b
? a
? b
? a
? h

```




```output1
1

```




```output2
2

```




```output3
0

```



## Note

<p>In the first test case after the first action it becomes clear that the selected letter is one of the following: <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i></span>. After the second action we can note that the selected letter is not <span class="tex-span"><i>a</i></span>. Valentin tells word "b" and doesn't get a shock. After that it is clear that the selected letter is <span class="tex-span"><i>c</i></span>, but Valentin pronounces the word <span class="tex-span"><i>cd</i></span> and gets an excessive electric shock. </p><p>In the second test case after the first two electric shocks we understand that the selected letter is <span class="tex-span"><i>e</i></span> or <span class="tex-span"><i>o</i></span>. Valentin tries some words consisting of these letters and after the second word it's clear that the selected letter is <span class="tex-span"><i>e</i></span>, but Valentin makes 3 more actions before he makes a correct hypothesis.</p><p>In the third example the selected letter can be uniquely determined only when Valentin guesses it, so he didn't get excessive electric shocks.</p>
