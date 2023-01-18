## Description

<div><p>Alice and Bob are playing a game with a string of characters, with Alice going first. The string consists <span class="tex-span"><i>n</i></span> characters, each of which is one of the first <span class="tex-span"><i>k</i></span> letters of the alphabet. On a player’s turn, they can either arbitrarily permute the characters in the words, or delete exactly one character in the word (if there is at least one character). In addition, their resulting word cannot have appeared before throughout the entire game. The player unable to make a valid move loses the game.</p><p>Given <span class="tex-span"><i>n</i>, <i>k</i>, <i>p</i></span>, find the number of words with exactly <span class="tex-span"><i>n</i></span> characters consisting of the first <span class="tex-span"><i>k</i></span> letters of the alphabet such that Alice will win if both Alice and Bob play optimally. Return this number modulo the prime number <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>The first line of input will contain three integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>, <span class="tex-span">10<sup class="upper-index">8</sup> ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup> + 100</span>, <span class="tex-span"><i>p</i></span> will be prime).</p></div><div class="output-specification"><p>Print a single integer, the number of winning words for Alice, modulo <span class="tex-span"><i>p</i></span>.</p></div>

## Input

<p>The first line of input will contain three integers <span class="tex-span"><i>n</i>, <i>k</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>, <span class="tex-span">10<sup class="upper-index">8</sup> ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup> + 100</span>, <span class="tex-span"><i>p</i></span> will be prime).</p>

## Output

<p>Print a single integer, the number of winning words for Alice, modulo <span class="tex-span"><i>p</i></span>.</p>





```input1
4 2 100000007

```




```output1
14

```



## Note

<p>There are 14 strings that that Alice can win with. For example, some strings are "bbaa" and "baaa". Alice will lose on strings like "aaaa" or "bbbb".</p>
