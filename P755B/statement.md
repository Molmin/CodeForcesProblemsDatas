## Description

<div><p>PolandBall is playing a game with EnemyBall. The rules are simple. Players have to say words in turns. You cannot say a word which was already said. PolandBall starts. The Ball which can't say a new word loses.</p><p>You're given two lists of words familiar to PolandBall and EnemyBall. Can you determine who wins the game, if both play optimally?</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— number of words PolandBall and EnemyBall know, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> strings follow, one per line&nbsp;— words familiar to PolandBall.</p><p>Then <span class="tex-span"><i>m</i></span> strings follow, one per line&nbsp;— words familiar to EnemyBall.</p><p>Note that one Ball <span class="tex-font-style-bf">cannot</span> know a word more than once (strings are unique), but some words <span class="tex-font-style-bf">can</span> be known by both players.</p><p>Each word is non-empty and consists of no more than <span class="tex-span">500</span> lowercase English alphabet letters.</p></div><div class="output-specification"><p>In a single line of print the answer&nbsp;— "<span class="tex-font-style-tt">YES</span>" if PolandBall wins and "<span class="tex-font-style-tt">NO</span>" otherwise. Both Balls play optimally.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>)&nbsp;— number of words PolandBall and EnemyBall know, respectively.</p><p>Then <span class="tex-span"><i>n</i></span> strings follow, one per line&nbsp;— words familiar to PolandBall.</p><p>Then <span class="tex-span"><i>m</i></span> strings follow, one per line&nbsp;— words familiar to EnemyBall.</p><p>Note that one Ball <span class="tex-font-style-bf">cannot</span> know a word more than once (strings are unique), but some words <span class="tex-font-style-bf">can</span> be known by both players.</p><p>Each word is non-empty and consists of no more than <span class="tex-span">500</span> lowercase English alphabet letters.</p>

## Output

<p>In a single line of print the answer&nbsp;— "<span class="tex-font-style-tt">YES</span>" if PolandBall wins and "<span class="tex-font-style-tt">NO</span>" otherwise. Both Balls play optimally.</p>





```input1
5 1
polandball
is
a
cool
character
nope

```




```input2
2 2
kremowka
wadowicka
kremowka
wiedenska

```




```input3
1 2
a
a
b

```




```output1
YES
```




```output2
YES
```




```output3
NO
```



## Note

<p>In the first example PolandBall knows much more words and wins effortlessly.</p><p>In the second example if PolandBall says <span class="tex-font-style-tt">kremowka</span> first, then EnemyBall cannot use that word anymore. EnemyBall can only say <span class="tex-font-style-tt">wiedenska</span>. PolandBall says <span class="tex-font-style-tt">wadowicka</span> and wins.</p>
