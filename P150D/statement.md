## Description

<div><p>Market stalls now have the long-awaited game The Colder Scrools V: Nvodsk. The game turned out to be difficult as hell and most students can't complete the last quest ("We don't go to Nvodsk..."). That threatened winter exams. The rector already started to wonder whether he should postpone the winter exams till April (in fact, he wanted to complete the quest himself). But all of a sudden a stranger appeared at the door of his office. "Good afternoon. My name is Chuck and I solve any problems" — he said.</p><p>And here they are sitting side by side but still they can't complete the mission. The thing is, to kill the final boss one should prove one's perfect skills in the art of managing letters. One should be a real magician to do that. And can you imagine what happens when magicians start competing... </p><p>But let's put it more formally: you are given a string and a set of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. You are allowed to choose any substring that is a palindrome and delete it. At that we receive some number of points equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>k</i></span> is the length of the deleted palindrome. For some <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> = </span>-1, which means that deleting palindrome strings of such length is <span class="tex-font-style-bf">forbidden</span>. After a substring is deleted, the remaining part "shifts together", that is, at no moment of time the string has gaps. The process is repeated while the string has at least one palindrome substring that can be deleted. All gained points are summed up.</p><p>Determine what maximum number of points can be earned.</p><p>"Oh" — said Chuck, raising from the chair, — "I used to love deleting palindromes, just like you, but one day I took an arrow in the Knee".</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ 150</span>) — the length of the string.</p><p>The second line contains exactly <span class="tex-span"><i>l</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span"> - 1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the points a player gains for deleting.</p><p>The third line contains exactly <span class="tex-span"><i>l</i></span> lowercase Latin letters — the original string from which a player can delete palindromes. The line contains no other characters apart from the newline character at the end of the string.</p></div><div class="output-specification"><p>Print a single number — the maximum number of points one can gain if he plays on the given string.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ 150</span>) — the length of the string.</p><p>The second line contains exactly <span class="tex-span"><i>l</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span"> - 1 ≤ <i>a</i><sub class="lower-index"><i>k</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the points a player gains for deleting.</p><p>The third line contains exactly <span class="tex-span"><i>l</i></span> lowercase Latin letters — the original string from which a player can delete palindromes. The line contains no other characters apart from the newline character at the end of the string.</p>

## Output

<p>Print a single number — the maximum number of points one can gain if he plays on the given string.</p>





```input1
7
-1 -1 -1 -1 -1 -1 -1
abacaba

```




```input2
7
1 -1 -1 -1 -1 -1 -1
abacaba

```




```input3
7
1 5 -1 -1 -1 -1 10
abacaba

```




```output1
0

```




```output2
7

```




```output3
16

```



## Note

<p>In the first sample we cannot delete any substring, so the best result is <span class="tex-span">0</span>. In the second sample we are allowed to delete only those palindromes whose length equals <span class="tex-span">1</span>, thus, if we delete the whole string, we get <span class="tex-span">7</span> points. In the third sample the optimal strategy is: first we delete character <span class="tex-font-style-tt">c</span>, then string <span class="tex-font-style-tt">aa</span>, then <span class="tex-font-style-tt">bb</span>, and the last one <span class="tex-font-style-tt">aa</span>. At that we get <span class="tex-span">1 + 3 * 5 = 16</span> points.</p>
