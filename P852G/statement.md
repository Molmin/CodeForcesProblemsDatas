## Description

<div><p>Smith wakes up at the side of a dirty, disused bathroom, his ankle chained to pipes. Next to him is tape-player with a hand-written message "Play Me". He finds a tape in his own back pocket. After putting the tape in the tape-player, he sees a key hanging from a ceiling, chained to some kind of a machine, which is connected to the terminal next to him. After pressing a Play button a rough voice starts playing from the tape:</p><p>"Listen up Smith. As you can see, you are in pretty tough situation and in order to escape, you have to solve a puzzle. </p><p>You are given <span class="tex-span"><i>N</i></span> strings which represent words. Each word is of the maximum length <span class="tex-span"><i>L</i></span> and consists of characters '<span class="tex-font-style-tt">a</span>'-'<span class="tex-font-style-tt">e</span>'. You are also given <span class="tex-span"><i>M</i></span> strings which represent patterns. Pattern is a string of length <span class="tex-span"> ≤  <i>L</i></span> and consists of characters '<span class="tex-font-style-tt">a</span>'-'<span class="tex-font-style-tt">e</span>' as well as the maximum 3 characters '<span class="tex-font-style-tt">?</span>'. Character '<span class="tex-font-style-tt">?</span>' is an unknown character, meaning it can be equal to any character 'a'-'e', or even an empty character. For each pattern find the number of words that matches with the given pattern. After solving it and typing the result in the terminal, the key will drop from the ceiling and you may escape. Let the game begin."</p><p>Help Smith escape.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤  100 000</span>, <span class="tex-span">1 ≤ <i>M</i> ≤  5000</span>), representing the number of words and patterns respectively.</p><p>The next <span class="tex-span"><i>N</i></span> lines represent each word, and after those <span class="tex-span"><i>N</i></span> lines, following <span class="tex-span"><i>M</i></span> lines represent each pattern. Each word and each pattern has a maximum length <span class="tex-span"><i>L</i></span> (<span class="tex-span">1 ≤ <i>L</i> ≤ 50</span>). Each pattern has no more that three characters '<span class="tex-font-style-tt">?</span>'. All other characters in words and patters are lowercase English letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">e</span>'.</p></div><div class="output-specification"><p>Output contains <span class="tex-span"><i>M</i></span> lines and each line consists of one integer, representing the number of words that match the corresponding pattern.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤  100 000</span>, <span class="tex-span">1 ≤ <i>M</i> ≤  5000</span>), representing the number of words and patterns respectively.</p><p>The next <span class="tex-span"><i>N</i></span> lines represent each word, and after those <span class="tex-span"><i>N</i></span> lines, following <span class="tex-span"><i>M</i></span> lines represent each pattern. Each word and each pattern has a maximum length <span class="tex-span"><i>L</i></span> (<span class="tex-span">1 ≤ <i>L</i> ≤ 50</span>). Each pattern has no more that three characters '<span class="tex-font-style-tt">?</span>'. All other characters in words and patters are lowercase English letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">e</span>'.</p>

## Output

<p>Output contains <span class="tex-span"><i>M</i></span> lines and each line consists of one integer, representing the number of words that match the corresponding pattern.</p>





```input1
3 1
abc
aec
ac
a?c

```




```output1
3

```



## Note

<p>If we switch '?' with 'b', 'e' and with empty character, we get 'abc', 'aec' and 'ac' respectively.</p>
