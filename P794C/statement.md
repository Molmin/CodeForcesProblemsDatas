## Description

<div><p>Oleg the client and Igor the analyst are good friends. However, sometimes they argue over little things. Recently, they started a new company, but they are having trouble finding a name for the company.</p><p>To settle this problem, they've decided to play a game. The company name will consist of <span class="tex-span"><i>n</i></span> letters. Oleg and Igor each have a set of <span class="tex-span"><i>n</i></span> letters (which might contain multiple copies of the same letter, the sets can be different). Initially, the company name is denoted by <span class="tex-span"><i>n</i></span> question marks. Oleg and Igor takes turns to play the game, Oleg moves first. In each turn, a player can choose one of the letters <span class="tex-span"><i>c</i></span> in his set and replace any of the question marks with <span class="tex-span"><i>c</i></span>. Then, a copy of the letter <span class="tex-span"><i>c</i></span> is removed from his set. The game ends when all the question marks has been replaced by some letter.</p><p>For example, suppose Oleg has the set of letters <span class="tex-span">{<i>i</i>, <i>o</i>, <i>i</i>}</span> and Igor has the set of letters <span class="tex-span">{<i>i</i>, <i>m</i>, <i>o</i>}</span>. One possible game is as follows :</p><p>Initially, the company name is <span class="tex-font-style-tt">???</span>.</p><p>Oleg replaces the second question mark with <span class="tex-font-style-tt">'i'</span>. The company name becomes <span class="tex-font-style-tt">?i?</span>. The set of letters Oleg have now is <span class="tex-span">{<i>i</i>, <i>o</i>}</span>.</p><p>Igor replaces the third question mark with <span class="tex-font-style-tt">'o'</span>. The company name becomes <span class="tex-font-style-tt">?io</span>. The set of letters Igor have now is <span class="tex-span">{<i>i</i>, <i>m</i>}</span>.</p><p>Finally, Oleg replaces the first question mark with <span class="tex-font-style-tt">'o'</span>. The company name becomes <span class="tex-font-style-tt">oio</span>. The set of letters Oleg have now is <span class="tex-span">{<i>i</i>}</span>.</p><p>In the end, the company name is <span class="tex-font-style-tt">oio</span>.</p><p>Oleg wants the company name to be as lexicographically small as possible while Igor wants the company name to be as lexicographically large as possible. What will be the company name if Oleg and Igor always play optimally?</p><p>A string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>...<i>s</i><sub class="lower-index"><i>m</i></sub></span> is called lexicographically smaller than a string <span class="tex-span"><i>t</i> = <i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>...<i>t</i><sub class="lower-index"><i>m</i></sub></span> (where <span class="tex-span"><i>s</i> ≠ <i>t</i></span>) if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub></span> where <span class="tex-span"><i>i</i></span> is the smallest index such that <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>. (so <span class="tex-span"><i>s</i><sub class="lower-index"><i>j</i></sub> = <i>t</i><sub class="lower-index"><i>j</i></sub></span> for all <span class="tex-span"><i>j</i> &lt; <i>i</i></span>)</p></div><div class="input-specification"><p>The first line of input contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>). All characters of the string are lowercase English letters. This string denotes the set of letters Oleg has initially.</p><p>The second line of input contains a string <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>n</i></span>. All characters of the string are lowercase English letters. This string denotes the set of letters Igor has initially.</p></div><div class="output-specification"><p>The output should contain a string of <span class="tex-span"><i>n</i></span> lowercase English letters, denoting the company name if Oleg and Igor plays optimally.</p></div>

## Input

<p>The first line of input contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>). All characters of the string are lowercase English letters. This string denotes the set of letters Oleg has initially.</p><p>The second line of input contains a string <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>n</i></span>. All characters of the string are lowercase English letters. This string denotes the set of letters Igor has initially.</p>

## Output

<p>The output should contain a string of <span class="tex-span"><i>n</i></span> lowercase English letters, denoting the company name if Oleg and Igor plays optimally.</p>





```input1
tinkoff
zscoder

```




```input2
xxxxxx
xxxxxx

```




```input3
ioi
imo

```




```output1
fzfsirk

```




```output2
xxxxxx

```




```output3
ioi

```



## Note

<p>One way to play optimally in the first sample is as follows :</p><ul><li> Initially, the company name is <span class="tex-font-style-tt">???????</span>.</li><li> Oleg replaces the first question mark with <span class="tex-font-style-tt">'f'</span>. The company name becomes <span class="tex-font-style-tt">f??????</span>.</li><li> Igor replaces the second question mark with <span class="tex-font-style-tt">'z'</span>. The company name becomes <span class="tex-font-style-tt">fz?????</span>.</li><li> Oleg replaces the third question mark with <span class="tex-font-style-tt">'f'</span>. The company name becomes <span class="tex-font-style-tt">fzf????</span>.</li><li> Igor replaces the fourth question mark with <span class="tex-font-style-tt">'s'</span>. The company name becomes <span class="tex-font-style-tt">fzfs???</span>.</li><li> Oleg replaces the fifth question mark with <span class="tex-font-style-tt">'i'</span>. The company name becomes <span class="tex-font-style-tt">fzfsi??</span>.</li><li> Igor replaces the sixth question mark with <span class="tex-font-style-tt">'r'</span>. The company name becomes <span class="tex-font-style-tt">fzfsir?</span>.</li><li> Oleg replaces the seventh question mark with <span class="tex-font-style-tt">'k'</span>. The company name becomes <span class="tex-font-style-tt">fzfsirk</span>.</li></ul><p>For the second sample, no matter how they play, the company name will always be <span class="tex-font-style-tt">xxxxxx</span>.</p>
