## Description

<div><p>Long ago, Vasily built a good fence at his country house. Vasily calls a fence <span class="tex-font-style-it">good</span>, if it is a series of <span class="tex-span"><i>n</i></span> consecutively fastened vertical boards of centimeter width, the height of each in centimeters is <span class="tex-font-style-bf">a positive integer</span>. The house owner remembers that the height of the <span class="tex-span"><i>i</i></span>-th board to the left is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Today Vasily decided to change the design of the fence he had built, by cutting his top connected part so that the fence remained good. The cut part should consist of only the upper parts of the boards, while the adjacent parts must be interconnected (share a non-zero length before cutting out of the fence).</p><p>You, as Vasily's curious neighbor, will count the number of possible ways to cut exactly one part as is described above. Two ways to cut a part are called distinct, if for the remaining fences there is such <span class="tex-span"><i>i</i></span>, that the height of the <span class="tex-span"><i>i</i></span>-th boards vary.</p><p>As Vasily's fence can be very high and long, get the remainder after dividing the required number of ways by <span class="tex-span">1 000 000 007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the number of boards in Vasily's fence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> equals the height of the <span class="tex-span"><i>i</i></span>-th board to the left.</p></div><div class="output-specification"><p>Print the remainder after dividing <span class="tex-span"><i>r</i></span> by <span class="tex-span">1 000 000 007</span>, where <span class="tex-span"><i>r</i></span> is the number of ways to cut exactly one connected part so that the part consisted of the upper parts of the boards and the remaining fence was <span class="tex-font-style-it">good</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000 000</span>)&nbsp;— the number of boards in Vasily's fence.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated numbers <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> equals the height of the <span class="tex-span"><i>i</i></span>-th board to the left.</p>

## Output

<p>Print the remainder after dividing <span class="tex-span"><i>r</i></span> by <span class="tex-span">1 000 000 007</span>, where <span class="tex-span"><i>r</i></span> is the number of ways to cut exactly one connected part so that the part consisted of the upper parts of the boards and the remaining fence was <span class="tex-font-style-it">good</span>.</p>





```input1
2
1 1

```




```input2
3
3 4 2

```




```output1
0

```




```output2
13

```



## Note

<p>From the fence from the first example it is impossible to cut exactly one piece so as the remaining fence was <span class="tex-font-style-it">good</span>.</p><p>All the possible variants of the resulting fence from the second sample look as follows (the grey shows the cut out part): </p><center> <img class="tex-graphics" src="file://e4rfDebV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
