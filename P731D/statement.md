## Description

<div><p>Archeologists have found a secret pass in the dungeon of one of the pyramids of Cycleland. To enter the treasury they have to open an unusual lock on the door. The lock consists of <span class="tex-span"><i>n</i></span> words, each consisting of some hieroglyphs. The wall near the lock has a round switch. Each rotation of this switch changes the hieroglyphs according to some rules. The instruction nearby says that the door will open only if words written on the lock would be sorted in <span class="tex-font-style-it">lexicographical order</span> (the definition of lexicographical comparison in given in notes section).</p><p>The rule that changes hieroglyphs is the following. One clockwise rotation of the round switch replaces each hieroglyph with the next hieroglyph in alphabet, i.e. hieroglyph <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>c</i> - 1</span>) is replaced with hieroglyph <span class="tex-span">(<i>x</i> + 1)</span>, and hieroglyph <span class="tex-span"><i>c</i></span> is replaced with hieroglyph <span class="tex-span">1</span>.</p><p>Help archeologist determine, how many clockwise rotations they should perform in order to open the door, or determine that this is impossible, i.e. no cyclic shift of the alphabet will make the sequence of words sorted lexicographically.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500 000</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of words, written on the lock, and the number of different hieroglyphs.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains the description of one word. The <span class="tex-span"><i>i</i></span>-th of these lines starts with integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 500 000</span>), that denotes the length of the <span class="tex-span"><i>i</i></span>-th word, followed by <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, 2</sub></span>, ..., <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>l</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>c</i></span>)&nbsp;— the indices of hieroglyphs that make up the <span class="tex-span"><i>i</i></span>-th word. Hieroglyph with index <span class="tex-span">1</span> is the smallest in the alphabet and with index <span class="tex-span"><i>c</i></span>&nbsp;— the biggest.</p><p>It's guaranteed, that the total length of all words doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>If it is possible to open the door by rotating the round switch, print integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ <i>c</i> - 1</span>) that defines the required number of clockwise rotations. If there are several valid <span class="tex-span"><i>x</i></span>, print any of them.</p><p>If it is impossible to open the door by this method, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500 000</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of words, written on the lock, and the number of different hieroglyphs.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contains the description of one word. The <span class="tex-span"><i>i</i></span>-th of these lines starts with integer <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 500 000</span>), that denotes the length of the <span class="tex-span"><i>i</i></span>-th word, followed by <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, 1</sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, 2</sub></span>, ..., <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i>, <i>l</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>c</i></span>)&nbsp;— the indices of hieroglyphs that make up the <span class="tex-span"><i>i</i></span>-th word. Hieroglyph with index <span class="tex-span">1</span> is the smallest in the alphabet and with index <span class="tex-span"><i>c</i></span>&nbsp;— the biggest.</p><p>It's guaranteed, that the total length of all words doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>If it is possible to open the door by rotating the round switch, print integer <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ <i>c</i> - 1</span>) that defines the required number of clockwise rotations. If there are several valid <span class="tex-span"><i>x</i></span>, print any of them.</p><p>If it is impossible to open the door by this method, print <span class="tex-span"> - 1</span>.</p>





```input1
4 3
2 3 2
1 1
3 2 3 1
4 2 3 1 2

```




```input2
2 5
2 4 2
2 4 2

```




```input3
4 4
1 2
1 3
1 4
1 2

```




```output1
1

```




```output2
0

```




```output3
-1

```



## Note

<p>Word <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> of length <span class="tex-span"><i>m</i></span> is <span class="tex-font-style-it">lexicographically not greater</span> than word <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>k</i></sub></span> of length <span class="tex-span"><i>k</i></span>, if one of two conditions hold: </p><ul> <li> at first position <span class="tex-span"><i>i</i></span>, such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, the character <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> goes earlier in the alphabet than character <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, i.e. <span class="tex-span"><i>a</i></span> has smaller character in the first position where they differ; </li><li> if there is no such position <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>m</i> ≤ <i>k</i></span>, i.e. the first word is a prefix of the second or two words are equal. </li></ul><p>The sequence of words is said to be sorted in lexicographical order if each word (except the last one) is lexicographically not greater than the next word.</p><p>In the first sample, after the round switch is rotated <span class="tex-span">1</span> position clockwise the words look as follows:</p><pre class="verbatim"><br>1 3<br>2<br>3 1 2<br>3 1 2 3<br></pre><p>In the second sample, words are already sorted in lexicographical order.</p><p>In the last sample, one can check that no shift of the alphabet will work.</p>
