## Description

<div><p>Arcady is a copywriter. His today's task is to type up an already well-designed story using his favorite text editor.</p><p>Arcady types words, punctuation signs and spaces one after another. Each letter and each sign (including line feed) requires one keyboard click in order to be printed. Moreover, when Arcady has a non-empty prefix of some word on the screen, the editor proposes a possible autocompletion for this word, more precisely one of the already printed words such that its prefix matches the currently printed prefix if this word is unique. For example, if Arcady has already printed «<span class="tex-font-style-tt">codeforces</span>», «<span class="tex-font-style-tt">coding</span>» and «<span class="tex-font-style-tt">codeforces</span>» once again, then there will be no autocompletion attempt for «<span class="tex-font-style-tt">cod</span>», but if he proceeds with «<span class="tex-font-style-tt">code</span>», the editor will propose «<span class="tex-font-style-tt">codeforces</span>».</p><p>With a single click Arcady can follow the editor's proposal, i.e. to transform the current prefix to it. Note that no additional symbols are printed after the autocompletion (no spaces, line feeds, etc). What is the minimum number of keyboard clicks Arcady has to perform to print the entire text, if he is not allowed to move the cursor or erase the already printed symbols?</p><p>A word here is a contiguous sequence of latin letters bordered by spaces, punctuation signs and line/text beginnings/ends. Arcady uses only lowercase letters. For example, there are 20 words in «<span class="tex-font-style-tt">it's well-known that tic-tac-toe is a paper-and-pencil game for two players, x and o.</span>».</p></div><div class="input-specification"><p>The only line contains Arcady's text, consisting only of lowercase latin letters, spaces, line feeds and the following punctuation signs: «<span class="tex-font-style-tt">.</span>», «<span class="tex-font-style-tt">,</span>», «<span class="tex-font-style-tt">?</span>», «<span class="tex-font-style-tt">!</span>», «<span class="tex-font-style-tt">'</span>» and «<span class="tex-font-style-tt">-</span>». The total amount of symbols doesn't exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>. It's guaranteed that all lines are non-empty.</p></div><div class="output-specification"><p>Print a single integer — the minimum number of clicks.</p></div>

## Input

<p>The only line contains Arcady's text, consisting only of lowercase latin letters, spaces, line feeds and the following punctuation signs: «<span class="tex-font-style-tt">.</span>», «<span class="tex-font-style-tt">,</span>», «<span class="tex-font-style-tt">?</span>», «<span class="tex-font-style-tt">!</span>», «<span class="tex-font-style-tt">'</span>» and «<span class="tex-font-style-tt">-</span>». The total amount of symbols doesn't exceed <span class="tex-span">3·10<sup class="upper-index">5</sup></span>. It's guaranteed that all lines are non-empty.</p>

## Output

<p>Print a single integer — the minimum number of clicks.</p>





```input1
snow affects sports such as skiing, snowboarding, and snowmachine travel.
snowboarding is a recreational activity and olympic and paralympic sport.

```




```input2
'co-co-co, codeforces?!'

```




```input3
thun-thun-thunder, thunder, thunder
thunder, thun-, thunder
thun-thun-thunder, thunder
thunder, feel the thunder
lightning then the thunder
thunder, feel the thunder
lightning then the thunder
thunder, thunder

```




```output1
141

```




```output2
25

```




```output3
183

```



## Note

<p>In sample case one it's optimal to use autocompletion for the first instance of «<span class="tex-font-style-tt">snowboarding</span>» after typing up «<span class="tex-font-style-tt">sn</span>» and for the second instance of «<span class="tex-font-style-tt">snowboarding</span>» after typing up «<span class="tex-font-style-tt">snowb</span>». This will save 7 clicks.</p><p>In sample case two it doesn't matter whether to use autocompletion or not.</p>
