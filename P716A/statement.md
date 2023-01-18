## Description

<div><p>ZS the Coder is coding on a crazy computer. If you don't type in a word for a <span class="tex-span"><i>c</i></span> consecutive seconds, everything you typed disappear! </p><p>More formally, if you typed a word at second <span class="tex-span"><i>a</i></span> and then the next word at second <span class="tex-span"><i>b</i></span>, then if <span class="tex-span"><i>b</i> - <i>a</i> ≤ <i>c</i></span>, just the new word is appended to other words on the screen. If <span class="tex-span"><i>b</i> - <i>a</i> &gt; <i>c</i></span>, then everything on the screen disappears and after that the word you have typed appears on the screen.</p><p>For example, if <span class="tex-span"><i>c</i> = 5</span> and you typed words at seconds <span class="tex-span">1, 3, 8, 14, 19, 20</span> then at the second <span class="tex-span">8</span> there will be <span class="tex-span">3</span> words on the screen. After that, everything disappears at the second <span class="tex-span">13</span> because nothing was typed. At the seconds <span class="tex-span">14</span> and <span class="tex-span">19</span> another two words are typed, and finally, at the second <span class="tex-span">20</span>, one more word is typed, and a total of <span class="tex-span">3</span> words remain on the screen.</p><p>You're given the times when ZS the Coder typed the words. Determine how many words remain on the screen after he finished typing everything.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of words ZS the Coder typed and the crazy computer delay respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub> &lt; <i>t</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>t</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the second when ZS the Coder typed the <span class="tex-span"><i>i</i></span>-th word.</p></div><div class="output-specification"><p>Print a single positive integer, the number of words that remain on the screen after all <span class="tex-span"><i>n</i></span> words was typed, in other words, at the second <span class="tex-span"><i>t</i><sub class="lower-index"><i>n</i></sub></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000, 1 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of words ZS the Coder typed and the crazy computer delay respectively.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub> &lt; <i>t</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>t</i><sub class="lower-index"><i>n</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the second when ZS the Coder typed the <span class="tex-span"><i>i</i></span>-th word.</p>

## Output

<p>Print a single positive integer, the number of words that remain on the screen after all <span class="tex-span"><i>n</i></span> words was typed, in other words, at the second <span class="tex-span"><i>t</i><sub class="lower-index"><i>n</i></sub></span>.</p>





```input1
6 5
1 3 8 14 19 20

```




```input2
6 1
1 3 5 7 9 10

```




```output1
3
```




```output2
2
```



## Note

<p>The first sample is already explained in the problem statement.</p><p>For the second sample, after typing the first word at the second <span class="tex-span">1</span>, it disappears because the next word is typed at the second <span class="tex-span">3</span> and <span class="tex-span">3 - 1 &gt; 1</span>. Similarly, only <span class="tex-span">1</span> word will remain at the second <span class="tex-span">9</span>. Then, a word is typed at the second <span class="tex-span">10</span>, so there will be two words on the screen, as the old word won't disappear because <span class="tex-span">10 - 9 ≤ 1</span>.</p>
