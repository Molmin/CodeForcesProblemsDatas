## Description

<div><p><span class="tex-font-style-bf">This problem is different with hard version only by constraints on total answers length</span></p><p><span class="tex-font-style-bf">It is an interactive problem</span></p><p>Venya joined a tour to the madhouse, in which orderlies play with patients the following game. Orderlies pick a string $s$ of length $n$, consisting only of lowercase English letters. The player can ask two types of queries: </p><ul> <li> <span class="tex-font-style-tt">? l r</span> – ask to list all substrings of $s[l..r]$. Substrings will be returned in random order, and in every substring, all characters will be randomly shuffled. </li><li> <span class="tex-font-style-tt">! s</span> – guess the string picked by the orderlies. This query can be asked exactly once, after that the game will finish. If the string is guessed correctly, the player wins, otherwise he loses. </li></ul><p>The player can ask <span class="tex-font-style-bf">no more than $3$ queries</span> of the first type.</p><p>To make it easier for the orderlies, there is an additional limitation: the total number of returned substrings in all queries of the first type must not exceed $(n+1)^2$.</p><p>Venya asked you to write a program, which will guess the string by interacting with the orderlies' program and acting by the game's rules.</p><p>Your program should immediately terminate after guessing the string using a query of the second type. In case your program guessed the string incorrectly, or it violated the game rules, it will receive verdict <span class="tex-font-style-tt">Wrong answer</span>.</p><p>Note that in every test case the string is fixed beforehand and will not change during the game, which means that the interactor is not adaptive.</p></div><div class="input-specification"><p>First line contains number $n$ ($1 \le n \le 100$)&nbsp;— the length of the picked string.</p></div><div><h2>Interaction</h2><p>You start the interaction by reading the number $n$.</p><p>To ask a query about a substring from $l$ to $r$ inclusively ($1 \le l \le r \le n$), you should output</p><p><span class="tex-font-style-tt">? l r</span></p><p>on a separate line. After this, all substrings of $s[l..r]$ will be returned in random order, each substring exactly once. In every returned substring all characters will be randomly shuffled.</p><p>In the case, if you ask an incorrect query, ask more than $3$ queries of the first type or there will be more than $(n+1)^2$ substrings returned in total, you will receive verdict <span class="tex-font-style-bf">Wrong answer</span>.</p><p>To guess the string $s$, you should output</p><p><span class="tex-font-style-tt">! s</span></p><p>on a separate line.</p><p>After printing each query, do not forget to flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To flush the output, you can use: </p><ul> <li> fflush(stdout) or cout.flush() in C++; </li><li> System.out.flush() in Java; </li><li> flush(output) in Pascal; </li><li> stdout.flush() in Python; </li><li> see documentation for other languages. </li></ul><p>If you received <span class="tex-font-style-tt">-</span> (dash) as an answer to any query, you need to terminate your program with exit code 0 (for example, by calling <span class="tex-font-style-tt">exit(0)</span>). This means that there was an error in the interaction protocol. If you don't terminate with exit code 0, you can receive any unsuccessful verdict.</p><p><span class="tex-font-style-bf">Hack format</span></p><p>To hack a solution, use the following format:</p><p>The first line should contain one integer $n$ ($1 \le n \le 100$)&nbsp;— the length of the string, and the following line should contain the string $s$.</p></div>

## Input

<p>First line contains number $n$ ($1 \le n \le 100$)&nbsp;— the length of the picked string.</p>





```input1
4

a
aa
a

cb
b
c

c
```




```output1
? 1 2

? 3 4

? 4 4

! aabc
```


