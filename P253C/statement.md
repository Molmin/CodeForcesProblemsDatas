## Description

<div><p>Vasya is pressing the keys on the keyboard reluctantly, squeezing out his ideas on the classical epos depicted in Homer's Odysseus... How can he explain to his literature teacher that he isn't going to become a writer? In fact, he is going to become a programmer. So, he would take great pleasure in writing a program, but none — in writing a composition.</p><p>As Vasya was fishing for a sentence in the dark pond of his imagination, he suddenly wondered: what is the least number of times he should push a key to shift the cursor from one position to another one?</p><p>Let's describe his question more formally: to type a text, Vasya is using the text editor. He has already written <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> characters (including spaces). If some line contains <span class="tex-span"><i>k</i></span> characters, then this line overall contains <span class="tex-span">(<i>k</i> + 1)</span> positions where the cursor can stand: before some character or after all characters (at the end of the line). Thus, the cursor's position is determined by a pair of integers <span class="tex-span">(<i>r</i>, <i>c</i>)</span>, where <span class="tex-span"><i>r</i></span> is the number of the line and <span class="tex-span"><i>c</i></span> is the cursor's position in the line (the positions are indexed starting from one from the beginning of the line).</p><p>Vasya doesn't use the mouse to move the cursor. He uses keys "Up", "Down", "Right" and "Left". When he pushes each of these keys, the cursor shifts in the needed direction. Let's assume that before the corresponding key is pressed, the cursor was located in the position <span class="tex-span">(<i>r</i>, <i>c</i>)</span>, then Vasya pushed key:</p><ul><li> "Up": if the cursor was located in the first line (<span class="tex-span"><i>r</i> = 1</span>), then it does not move. Otherwise, it moves to the previous line (with number <span class="tex-span"><i>r</i> - 1</span>), to the same position. At that, if the previous line was short, that is, the cursor couldn't occupy position <span class="tex-span"><i>c</i></span> there, the cursor moves to the last position of the line with number <span class="tex-span"><i>r</i> - 1</span>;</li><li> "Down": if the cursor was located in the last line (<span class="tex-span"><i>r</i> = <i>n</i></span>), then it does not move. Otherwise, it moves to the next line (with number <span class="tex-span"><i>r</i> + 1</span>), to the same position. At that, if the next line was short, that is, the cursor couldn't occupy position <span class="tex-span"><i>c</i></span> there, the cursor moves to the last position of the line with number <span class="tex-span"><i>r</i> + 1</span>;</li><li> "Right": if the cursor can move to the right in this line (<span class="tex-span"><i>c</i> &lt; <i>a</i><sub class="lower-index"><i>r</i></sub> + 1</span>), then it moves to the right (to position <span class="tex-span"><i>c</i> + 1</span>). Otherwise, it is located at the end of the line and doesn't move anywhere when Vasya presses the "Right" key;</li><li> "Left": if the cursor can move to the left in this line (<span class="tex-span"><i>c</i> &gt; 1</span>), then it moves to the left (to position <span class="tex-span"><i>c</i> - 1</span>). Otherwise, it is located at the beginning of the line and doesn't move anywhere when Vasya presses the "Left" key.</li></ul><p>You've got the number of lines in the text file and the number of characters, written in each line of this file. Find the least number of times Vasya should push the keys, described above, to shift the cursor from position <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to position <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of lines in the file. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), separated by single spaces. The third line contains four integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index">1</sub></sub> + 1, 1 ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index">2</sub></sub> + 1</span>).</p></div><div class="output-specification"><p>Print a single integer — the minimum number of times Vasya should push a key to move the cursor from position <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to position <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of lines in the file. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>), separated by single spaces. The third line contains four integers <span class="tex-span"><i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index">1</sub>, <i>r</i><sub class="lower-index">2</sub> ≤ <i>n</i>, 1 ≤ <i>c</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index">1</sub></sub> + 1, 1 ≤ <i>c</i><sub class="lower-index">2</sub> ≤ <i>a</i><sub class="lower-index"><i>r</i><sub class="lower-index">2</sub></sub> + 1</span>).</p>

## Output

<p>Print a single integer — the minimum number of times Vasya should push a key to move the cursor from position <span class="tex-span">(<i>r</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> to position <span class="tex-span">(<i>r</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">2</sub>)</span>.</p>





```input1
4
2 1 6 4
3 4 4 2

```




```input2
4
10 5 6 4
1 11 4 2

```




```input3
3
10 1 10
1 10 1 1

```




```output1
3

```




```output2
6

```




```output3
3

```



## Note

<p>In the first sample the editor contains four lines. Let's represent the cursor's possible positions in the line as numbers. Letter <span class="tex-span"><i>s</i></span> represents the cursor's initial position, letter <span class="tex-span"><i>t</i></span> represents the last one. Then all possible positions of the cursor in the text editor are described by the following table.</p><p><span class="tex-font-style-tt">123</span></p><p><span class="tex-font-style-tt">12</span></p><p><span class="tex-font-style-tt">123s567</span></p><p><span class="tex-font-style-tt">1t345</span></p><p>One of the possible answers in the given sample is: "Left", "Down", "Left".</p>
