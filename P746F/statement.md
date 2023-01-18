## Description

<div><p>Sasha reaches the work by car. It takes exactly <span class="tex-span"><i>k</i></span> minutes. On his way he listens to music. All songs in his playlist go one by one, after listening to the <span class="tex-span"><i>i</i></span>-th song Sasha gets a pleasure which equals <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th song lasts for <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> minutes. </p><p>Before the beginning of his way Sasha turns on some song <span class="tex-span"><i>x</i></span> and then he listens to the songs one by one: at first, the song <span class="tex-span"><i>x</i></span>, then the song <span class="tex-span">(<i>x</i> + 1)</span>, then the song number <span class="tex-span">(<i>x</i> + 2)</span>, and so on. He listens to songs until he reaches the work or until he listens to the last song in his playlist. </p><p>Sasha can listen to each song to the end or <span class="tex-font-style-it">partly</span>.</p><p>In the second case he listens to the song for integer number of minutes, at least half of the song's length. Formally, if the length of the song equals <span class="tex-span"><i>d</i></span> minutes, Sasha listens to it for no less than <img align="middle" class="tex-formula" src="file://p0kivOe1.png" style="max-width: 100.0%;max-height: 100.0%;"> minutes, then he immediately switches it to the next song (if there is such). For example, if the length of the song which Sasha wants to <span class="tex-font-style-it">partly</span> listen to, equals <span class="tex-span">5</span> minutes, then he should listen to it for at least <span class="tex-span">3</span> minutes, if the length of the song equals <span class="tex-span">8</span> minutes, then he should listen to it for at least <span class="tex-span">4</span> minutes.</p><p>It takes no time to switch a song.</p><p>Sasha wants to listen <span class="tex-font-style-it">partly</span> no more than <span class="tex-span"><i>w</i></span> songs. If the last listened song plays for less than half of its length, then Sasha doesn't get pleasure from it and that song is not included to the list of <span class="tex-font-style-it">partly</span> listened songs. It is not allowed to skip songs. A pleasure from a song does not depend on the listening mode, for the <span class="tex-span"><i>i</i></span>-th song this value equals <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Help Sasha to choose such <span class="tex-span"><i>x</i></span> and no more than <span class="tex-span"><i>w</i></span> songs for <span class="tex-font-style-it">partial</span> listening to get the maximum pleasure. Write a program to find the maximum pleasure Sasha can get from the listening to the songs on his way to the work.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>w</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of songs in the playlist, the number of songs Sasha can listen to <span class="tex-font-style-it">partly</span> and time in minutes which Sasha needs to reach work. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals the pleasure Sasha gets after listening to the <span class="tex-span"><i>i</i></span>-th song.</p><p>The third line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals the length of the <span class="tex-span"><i>i</i></span>-th song in minutes.</p></div><div class="output-specification"><p>Print the maximum pleasure Sasha can get after listening to the songs on the way to work. </p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>w</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of songs in the playlist, the number of songs Sasha can listen to <span class="tex-font-style-it">partly</span> and time in minutes which Sasha needs to reach work. </p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals the pleasure Sasha gets after listening to the <span class="tex-span"><i>i</i></span>-th song.</p><p>The third line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">2 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals the length of the <span class="tex-span"><i>i</i></span>-th song in minutes.</p>

## Output

<p>Print the maximum pleasure Sasha can get after listening to the songs on the way to work. </p>





```input1
7 2 11
3 4 3 5 1 4 6
7 7 3 6 5 3 9

```




```input2
8 4 20
5 6 4 3 7 5 4 1
10 12 5 12 14 8 5 8

```




```input3
1 1 5
6
9

```




```input4
1 1 3
4
7

```




```output1
12

```




```output2
19

```




```output3
6

```




```output4
0

```



## Note

<p>In the first example Sasha needs to start listening from the song number <span class="tex-span">2</span>. He should listen to it <span class="tex-font-style-it">partly</span> (for <span class="tex-span">4</span> minutes), then listen to the song number <span class="tex-span">3</span> to the end (for <span class="tex-span">3</span> minutes) and then <span class="tex-font-style-it">partly</span> listen to the song number <span class="tex-span">4</span> (for <span class="tex-span">3</span> minutes). After listening to these songs Sasha will get pleasure which equals <span class="tex-span">4 + 3 + 5 = 12</span>. Sasha will not have time to listen to the song number <span class="tex-span">5</span> because he will spend <span class="tex-span">4 + 3 + 3 = 10</span> minutes listening to songs number <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span> and only <span class="tex-span">1</span> minute is left after that. </p>
