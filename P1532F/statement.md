## Description

<div><p>Ivan wants to play a game with you. He picked some string $s$ of length $n$ consisting only of lowercase Latin letters. </p><p>You don't know this string. Ivan has informed you about all its improper prefixes and suffixes (i.e. prefixes and suffixes of lengths from $1$ to $n-1$), but he didn't tell you which strings are prefixes and which are suffixes.</p><p>Ivan wants you to guess which of the given $2n-2$ strings are prefixes of the given string and which are suffixes. It may be impossible to guess the string Ivan picked (since multiple strings may give the same set of suffixes and prefixes), but Ivan will accept your answer if there is at least one string that is consistent with it. Let the game begin!</p></div><div class="input-specification"><p>The first line of the input contains one integer number $n$ ($2 \le n \le 100$) — the length of the guessed string $s$.</p><p>The next $2n-2$ lines are contain prefixes and suffixes, one per line. Each of them is the string of length from $1$ to $n-1$ consisting only of lowercase Latin letters. They can be given in arbitrary order.</p><p>It is guaranteed that there are exactly $2$ strings of each length from $1$ to $n-1$. It is also guaranteed that these strings are prefixes and suffixes of some existing string of length $n$.</p></div><div class="output-specification"><p>Print one string of length $2n-2$ — the string consisting only of characters '<span class="tex-font-style-tt">P</span>' and '<span class="tex-font-style-tt">S</span>'. The number of characters '<span class="tex-font-style-tt">P</span>' should be equal to the number of characters '<span class="tex-font-style-tt">S</span>'. The $i$-th character of this string should be '<span class="tex-font-style-tt">P</span>' if the $i$-th of the input strings is the prefix and '<span class="tex-font-style-tt">S</span>' otherwise.</p><p>If there are several possible answers, you can print <span class="tex-font-style-bf">any</span>.</p></div>

## Input

<p>The first line of the input contains one integer number $n$ ($2 \le n \le 100$) — the length of the guessed string $s$.</p><p>The next $2n-2$ lines are contain prefixes and suffixes, one per line. Each of them is the string of length from $1$ to $n-1$ consisting only of lowercase Latin letters. They can be given in arbitrary order.</p><p>It is guaranteed that there are exactly $2$ strings of each length from $1$ to $n-1$. It is also guaranteed that these strings are prefixes and suffixes of some existing string of length $n$.</p>

## Output

<p>Print one string of length $2n-2$ — the string consisting only of characters '<span class="tex-font-style-tt">P</span>' and '<span class="tex-font-style-tt">S</span>'. The number of characters '<span class="tex-font-style-tt">P</span>' should be equal to the number of characters '<span class="tex-font-style-tt">S</span>'. The $i$-th character of this string should be '<span class="tex-font-style-tt">P</span>' if the $i$-th of the input strings is the prefix and '<span class="tex-font-style-tt">S</span>' otherwise.</p><p>If there are several possible answers, you can print <span class="tex-font-style-bf">any</span>.</p>





```input1
5
ba
a
abab
a
aba
baba
ab
aba
```




```input2
3
a
aa
aa
a
```




```input3
2
a
c
```




```output1
SPPSPSPS
```




```output2
PPSS
```




```output3
PS
```



## Note

<p>The only string which Ivan can guess in the first example is "<span class="tex-font-style-tt">ababa</span>".</p><p>The only string which Ivan can guess in the second example is "<span class="tex-font-style-tt">aaa</span>". Answers "<span class="tex-font-style-tt">SPSP</span>", "<span class="tex-font-style-tt">SSPP</span>" and "<span class="tex-font-style-tt">PSPS</span>" are also acceptable.</p><p>In the third example Ivan can guess the string "<span class="tex-font-style-tt">ac</span>" or the string "<span class="tex-font-style-tt">ca</span>". The answer "<span class="tex-font-style-tt">SP</span>" is also acceptable.</p>
