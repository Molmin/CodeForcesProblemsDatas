## Description

<div><p>Vasya has a pack of <span class="tex-span">54</span> cards (<span class="tex-span">52</span> standard cards and <span class="tex-span">2</span> distinct jokers). That is all he has at the moment. Not to die from boredom, Vasya plays Solitaire with them.</p><p>Vasya lays out <span class="tex-span"><i>nm</i></span> cards as a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span>. If there are jokers among them, then Vasya should change them with some of the rest of <span class="tex-span">54 - <i>nm</i></span> cards (which are not layed out) so that there were no jokers left. Vasya can pick the cards to replace the jokers arbitrarily. Remember, that each card presents in pack exactly once (i. e. <span class="tex-font-style-bf">in a single copy</span>). Vasya tries to perform the replacements so that the solitaire was <span class="tex-font-style-it">solved</span>.</p><p>Vasya thinks that the solitaire is solved if after the jokers are replaced, there exist two non-overlapping squares <span class="tex-span">3 × 3</span>, inside each of which all the cards either have the same suit, or pairwise different ranks.</p><p>Determine by the initial position whether the solitaire can be solved or not. If it can be solved, show the way in which it is possible.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 17</span>, <span class="tex-span"><i>n</i> × <i>m</i> ≤ 52</span>). Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> words each. Each word consists of two letters. The jokers are defined as "<span class="tex-font-style-tt">J1</span>" and "<span class="tex-font-style-tt">J2</span>" correspondingly. For the rest of the cards, the first letter stands for the rank and the second one — for the suit. The possible ranks are: "<span class="tex-font-style-tt">2</span>", "<span class="tex-font-style-tt">3</span>", "<span class="tex-font-style-tt">4</span>", "<span class="tex-font-style-tt">5</span>", "<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">7</span>", "<span class="tex-font-style-tt">8</span>", "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">J</span>", "<span class="tex-font-style-tt">Q</span>", "<span class="tex-font-style-tt">K</span>" and "<span class="tex-font-style-tt">A</span>". The possible suits are: "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">H</span>" and "<span class="tex-font-style-tt">S</span>". All the cards are different.</p></div><div class="output-specification"><p>If the Solitaire can be solved, print on the first line "<span class="tex-font-style-tt">Solution exists.</span>" without the quotes. On the second line print in what way the jokers can be replaced. Three variants are possible:</p><ul> <li> "<span class="tex-font-style-tt">There are no jokers.</span>", if there are no jokers in the input data.</li><li> "<span class="tex-font-style-tt">Replace J<span class="tex-span"><i>x</i></span> with <span class="tex-span"><i>y</i></span>.</span>", if there is one joker. <span class="tex-span"><i>x</i></span> is its number, and <span class="tex-span"><i>y</i></span> is the card it should be replaced with.</li><li> "<span class="tex-font-style-tt">Replace J1 with <span class="tex-span"><i>x</i></span> and J2 with <span class="tex-span"><i>y</i></span>.</span>", if both jokers are present in the input data. <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> here represent distinct cards with which one should replace the first and the second jokers correspondingly.</li></ul><p>On the third line print the coordinates of the upper left corner of the first square <span class="tex-span">3 × 3</span> in the format "<span class="tex-font-style-tt">Put the first square to (<span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span>).</span>", where <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> are the row and the column correspondingly. In the same manner print on the fourth line the coordinates of the second square <span class="tex-span">3 × 3</span> in the format "<span class="tex-font-style-tt">Put the second square to (<span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span>).</span>".</p><p>If there are several solutions to that problem, print any of them.</p><p>If there are no solutions, print of the single line "<span class="tex-font-style-tt">No solution.</span>" without the quotes.</p><p>See the samples to understand the output format better.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 17</span>, <span class="tex-span"><i>n</i> × <i>m</i> ≤ 52</span>). Next <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> words each. Each word consists of two letters. The jokers are defined as "<span class="tex-font-style-tt">J1</span>" and "<span class="tex-font-style-tt">J2</span>" correspondingly. For the rest of the cards, the first letter stands for the rank and the second one — for the suit. The possible ranks are: "<span class="tex-font-style-tt">2</span>", "<span class="tex-font-style-tt">3</span>", "<span class="tex-font-style-tt">4</span>", "<span class="tex-font-style-tt">5</span>", "<span class="tex-font-style-tt">6</span>", "<span class="tex-font-style-tt">7</span>", "<span class="tex-font-style-tt">8</span>", "<span class="tex-font-style-tt">9</span>", "<span class="tex-font-style-tt">T</span>", "<span class="tex-font-style-tt">J</span>", "<span class="tex-font-style-tt">Q</span>", "<span class="tex-font-style-tt">K</span>" and "<span class="tex-font-style-tt">A</span>". The possible suits are: "<span class="tex-font-style-tt">C</span>", "<span class="tex-font-style-tt">D</span>", "<span class="tex-font-style-tt">H</span>" and "<span class="tex-font-style-tt">S</span>". All the cards are different.</p>

## Output

<p>If the Solitaire can be solved, print on the first line "<span class="tex-font-style-tt">Solution exists.</span>" without the quotes. On the second line print in what way the jokers can be replaced. Three variants are possible:</p><ul> <li> "<span class="tex-font-style-tt">There are no jokers.</span>", if there are no jokers in the input data.</li><li> "<span class="tex-font-style-tt">Replace J<span class="tex-span"><i>x</i></span> with <span class="tex-span"><i>y</i></span>.</span>", if there is one joker. <span class="tex-span"><i>x</i></span> is its number, and <span class="tex-span"><i>y</i></span> is the card it should be replaced with.</li><li> "<span class="tex-font-style-tt">Replace J1 with <span class="tex-span"><i>x</i></span> and J2 with <span class="tex-span"><i>y</i></span>.</span>", if both jokers are present in the input data. <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> here represent distinct cards with which one should replace the first and the second jokers correspondingly.</li></ul><p>On the third line print the coordinates of the upper left corner of the first square <span class="tex-span">3 × 3</span> in the format "<span class="tex-font-style-tt">Put the first square to (<span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span>).</span>", where <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>c</i></span> are the row and the column correspondingly. In the same manner print on the fourth line the coordinates of the second square <span class="tex-span">3 × 3</span> in the format "<span class="tex-font-style-tt">Put the second square to (<span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>c</i></span>).</span>".</p><p>If there are several solutions to that problem, print any of them.</p><p>If there are no solutions, print of the single line "<span class="tex-font-style-tt">No solution.</span>" without the quotes.</p><p>See the samples to understand the output format better.</p>





```input1
4 6
2S 3S 4S 7S 8S AS
5H 6H 7H 5S TC AC
8H 9H TH 7C 8C 9C
2D 2C 3C 4C 5C 6C

```




```input2
4 6
2S 3S 4S 7S 8S AS
5H 6H 7H J1 TC AC
8H 9H TH 7C 8C 9C
2D 2C 3C 4C 5C 6C

```




```input3
4 6
2S 3S 4S 7S 8S AS
5H 6H 7H QC TC AC
8H 9H TH 7C 8C 9C
2D 2C 3C 4C 5C 6C

```




```output1
No solution.
```




```output2
Solution exists.
Replace J1 with 2H.
Put the first square to (1, 1).
Put the second square to (2, 4).

```




```output3
Solution exists.
There are no jokers.
Put the first square to (1, 1).
Put the second square to (2, 4).

```



## Note

<p>The pretests cover all the possible output formats.</p>
