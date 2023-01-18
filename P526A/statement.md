## Description

<div><p><span class="tex-font-style-it">In this problem you will meet the simplified model of game King of Thieves</span>.</p><p>In a new ZeptoLab game called "King of Thieves" your aim is to reach a chest with gold by controlling your character, avoiding traps and obstacles on your way.</p><center> <img class="tex-graphics" src="file://nCuqkg4z.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>An interesting feature of the game is that you can design your own levels that will be available to other players. Let's consider the following simple design of a level.</p><p>A dungeon consists of <span class="tex-span"><i>n</i></span> segments located at a same vertical level, each segment is either a platform that character can stand on, or a pit with a trap that makes player lose if he falls into it. All segments have the same length, platforms on the scheme of the level are represented as <span class="tex-font-style-tt">'*'</span> and pits are represented as <span class="tex-font-style-tt">'.'</span>. </p><p>One of things that affects speedrun characteristics of the level is a possibility to perform a series of consecutive jumps of the same length. More formally, when the character is on the platform number <span class="tex-span"><i>i</i><sub class="lower-index">1</sub></span>, he can make a sequence of jumps through the platforms <span class="tex-span"><i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub></span>, if <span class="tex-span"><i>i</i><sub class="lower-index">2</sub> - <i>i</i><sub class="lower-index">1</sub> = <i>i</i><sub class="lower-index">3</sub> - <i>i</i><sub class="lower-index">2</sub> = ... = <i>i</i><sub class="lower-index"><i>k</i></sub> - <i>i</i><sub class="lower-index"><i>k</i> - 1</sub></span>. Of course, all segments <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ... <i>i</i><sub class="lower-index"><i>k</i></sub></span> should be exactly the platforms, not pits. </p><p>Let's call a level to be <span class="tex-font-style-it">good</span> if you can perform a sequence of <span class="tex-font-style-bf">four</span> jumps of the same length or in the other words there must be a sequence <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index">5</sub></span>, consisting of <span class="tex-font-style-bf">five</span> platforms so that the intervals between consecutive platforms are of the same length. Given the scheme of the level, check if it is good.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of segments on the level.</p><p>Next line contains the scheme of the level represented as a string of <span class="tex-span"><i>n</i></span> characters <span class="tex-font-style-tt">'*'</span> and <span class="tex-font-style-tt">'.'</span>.</p></div><div class="output-specification"><p>If the level is <span class="tex-font-style-it">good</span>, print the word <span class="tex-font-style-tt">"yes"</span> (without the quotes), otherwise print the word <span class="tex-font-style-tt">"no"</span> (without the quotes).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of segments on the level.</p><p>Next line contains the scheme of the level represented as a string of <span class="tex-span"><i>n</i></span> characters <span class="tex-font-style-tt">'*'</span> and <span class="tex-font-style-tt">'.'</span>.</p>

## Output

<p>If the level is <span class="tex-font-style-it">good</span>, print the word <span class="tex-font-style-tt">"yes"</span> (without the quotes), otherwise print the word <span class="tex-font-style-tt">"no"</span> (without the quotes).</p>





```input1
16
.**.*..*.***.**.

```




```input2
11
.*.*...*.*.

```




```output1
yes
```




```output2
no
```



## Note

<p>In the first sample test you may perform a sequence of jumps through platforms <span class="tex-span">2, 5, 8, 11, 14</span>.</p>
