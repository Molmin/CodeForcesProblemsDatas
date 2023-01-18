## Description

<div><center> <img class="tex-graphics" src="file://eMOtx6f9.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Slastyona and her loyal dog Pushok are playing a meaningless <span class="tex-font-style-it">game</span> that is indeed very interesting.</p><p>The <span class="tex-font-style-it">game</span> consists of multiple <span class="tex-font-style-it">rounds</span>. Its rules are very simple: in each round, a natural number <span class="tex-span"><i>k</i></span> is chosen. Then, the one who says (or barks) it faster than the other wins the <span class="tex-font-style-it">round</span>. After that, the winner's score is multiplied by <span class="tex-span"><i>k</i><sup class="upper-index">2</sup></span>, and the loser's score is multiplied by <span class="tex-span"><i>k</i></span>. In the beginning of the <span class="tex-font-style-it">game</span>, both Slastyona and Pushok have scores equal to one.</p><p>Unfortunately, Slastyona had lost her notepad where the history of all <span class="tex-span"><i>n</i></span> <span class="tex-font-style-it">games</span> was recorded. She managed to recall the final results for each games, though, but all of her memories of them are vague. Help Slastyona verify their correctness, or, to put it another way, for each given pair of scores determine whether it was possible for a game to finish with such result or not.</p></div><div class="input-specification"><p>In the first string, the number of games <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 350000)</span> is given.</p><p>Each <span class="tex-font-style-it">game</span> is represented by a pair of scores <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;– the results of Slastyona and Pushok, correspondingly.</p></div><div class="output-specification"><p>For each pair of scores, answer "<span class="tex-font-style-tt">Yes</span>" if it's possible for a game to finish with given score, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in arbitrary case (upper or lower).</p></div>

## Input

<p>In the first string, the number of games <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 350000)</span> is given.</p><p>Each <span class="tex-font-style-it">game</span> is represented by a pair of scores <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup>)</span>&nbsp;– the results of Slastyona and Pushok, correspondingly.</p>

## Output

<p>For each pair of scores, answer "<span class="tex-font-style-tt">Yes</span>" if it's possible for a game to finish with given score, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can output each letter in arbitrary case (upper or lower).</p>





```input1
6
2 4
75 45
8 8
16 16
247 994
1000000000 1000000

```




```output1
Yes
Yes
Yes
No
No
Yes

```



## Note

<p>First <span class="tex-font-style-it">game</span> might have been consisted of one round, in which the number <span class="tex-span">2</span> would have been chosen and Pushok would have won.</p><p>The second <span class="tex-font-style-it">game</span> needs exactly two rounds to finish with such result: in the first one, Slastyona would have said the number <span class="tex-span">5</span>, and in the second one, Pushok would have barked the number <span class="tex-span">3</span>.</p>
