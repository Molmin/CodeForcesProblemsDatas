## Description

<div><p>The game of Egg Roulette is played between two players. Initially <span class="tex-span">2<i>R</i></span> raw eggs and <span class="tex-span">2<i>C</i></span> cooked eggs are placed randomly into a carton. The shells are left on so there is no way to distinguish a raw egg from a cooked egg. One at a time, a player will select an egg, and then smash the egg on his/her forehead. If the egg was cooked, not much happens, but if the egg was raw, it will make quite the mess. This continues until one player has broken <span class="tex-span"><i>R</i></span> raw eggs, at which point that player is declared the loser and the other player wins.</p><p>The order in which players take turns can be described as a string of '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">B</span>' characters, where the <span class="tex-span"><i>i</i></span>-th character tells which player should choose the <span class="tex-span"><i>i</i></span>-th egg. Traditionally, players take turns going one after the other. That is, they follow the ordering "<span class="tex-font-style-tt">ABABAB...</span>". This isn't very fair though, because the second player will win more often than the first. We'd like you to find a better ordering for the players to take their turns. Let's define the unfairness of an ordering as the absolute difference between the first player's win probability and the second player's win probability. We're interested in orderings that minimize the unfairness. We only consider an ordering valid if it contains the same number of '<span class="tex-font-style-tt">A</span>'s as '<span class="tex-font-style-tt">B</span>'s.</p><p>You will also be given a string <span class="tex-span"><i>S</i></span> of length <span class="tex-span">2(<i>R</i> + <i>C</i>)</span> containing only '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', and '<span class="tex-font-style-tt">?</span>' characters. An ordering is said to match <span class="tex-span"><i>S</i></span> if it only differs from <span class="tex-span"><i>S</i></span> in positions where <span class="tex-span"><i>S</i></span> contains a '<span class="tex-font-style-tt">?</span>'. Of the valid orderings that minimize unfairness, how many match <span class="tex-span"><i>S</i></span>?</p></div><div class="input-specification"><p>The first line of input will contain integers <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>C</i></span> <span class="tex-span">(1 ≤ <i>R</i>, <i>C</i> ≤ 20, <i>R</i> + <i>C</i> ≤ 30)</span>.</p><p>The second line of input will contain the string <span class="tex-span"><i>S</i></span> of length <span class="tex-span">2(<i>R</i> + <i>C</i>)</span> consisting only of characters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">?</span>'.</p></div><div class="output-specification"><p>Print the number of valid orderings that minimize unfairness and match <span class="tex-span"><i>S</i></span>.</p></div>

## Input

<p>The first line of input will contain integers <span class="tex-span"><i>R</i></span> and <span class="tex-span"><i>C</i></span> <span class="tex-span">(1 ≤ <i>R</i>, <i>C</i> ≤ 20, <i>R</i> + <i>C</i> ≤ 30)</span>.</p><p>The second line of input will contain the string <span class="tex-span"><i>S</i></span> of length <span class="tex-span">2(<i>R</i> + <i>C</i>)</span> consisting only of characters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">?</span>'.</p>

## Output

<p>Print the number of valid orderings that minimize unfairness and match <span class="tex-span"><i>S</i></span>.</p>





```input1
1 1
??BB

```




```input2
2 4
?BA??B??A???

```




```input3
4 14
????A??BB?????????????AB????????????

```




```output1
0

```




```output2
1

```




```output3
314

```



## Note

<p>In the first test case, the minimum unfairness is <span class="tex-span">0</span>, and the orderings that achieve it are "<span class="tex-font-style-tt">ABBA</span>" and "<span class="tex-font-style-tt">BAAB</span>", neither of which match <span class="tex-span"><i>S</i></span>. Note that an ordering such as "<span class="tex-font-style-tt">ABBB</span>" would also have an unfairness of <span class="tex-span">0</span>, but is invalid because it does not contain the same number of '<span class="tex-font-style-tt">A</span>'s as '<span class="tex-font-style-tt">B</span>'s.</p><p>In the second example, the only matching ordering is "<span class="tex-font-style-tt">BBAAABABABBA</span>".</p>
