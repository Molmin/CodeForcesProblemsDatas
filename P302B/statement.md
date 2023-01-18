## Description

<div><p>Eugeny loves listening to music. He has <span class="tex-span"><i>n</i></span> songs in his play list. We know that song number <span class="tex-span"><i>i</i></span> has the duration of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> minutes. Eugeny listens to each song, perhaps more than once. He listens to song number <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> times. Eugeny's play list is organized as follows: first song number <span class="tex-span">1</span> plays <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span> times, then song number <span class="tex-span">2</span> plays <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span> times, <span class="tex-span">...</span>, in the end the song number <span class="tex-span"><i>n</i></span> plays <span class="tex-span"><i>c</i><sub class="lower-index"><i>n</i></sub></span> times.</p><p>Eugeny took a piece of paper and wrote out <span class="tex-span"><i>m</i></span> moments of time when he liked a song. Now for each such moment he wants to know the number of the song that played at that moment. The moment <span class="tex-span"><i>x</i></span> means that Eugeny wants to know which song was playing during the <span class="tex-span"><i>x</i></span>-th minute of his listening to the play list.</p><p>Help Eugeny and calculate the required numbers of songs.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>n</i></span> lines contain pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the description of the play list. It is guaranteed that the play list's total duration doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> <img align="middle" class="tex-formula" src="file://R6q3mTjY.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The next line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>m</i></sub></span>, that describe the moments Eugeny has written out. It is guaranteed that there isn't such moment of time <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, when the music doesn't play any longer. It is guaranteed that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> <span class="tex-span">(<i>i</i> &lt; <i>m</i>)</span>.</p><p>The moment of time <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> means that Eugeny wants to know which song was playing during the <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th munite from the start of listening to the playlist.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th number must equal the number of the song that was playing during the <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th minute after Eugeny started listening to the play list.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The next <span class="tex-span"><i>n</i></span> lines contain pairs of integers. The <span class="tex-span"><i>i</i></span>-th line contains integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the description of the play list. It is guaranteed that the play list's total duration doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span> <img align="middle" class="tex-formula" src="file://R6q3mTjY.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>The next line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>m</i></sub></span>, that describe the moments Eugeny has written out. It is guaranteed that there isn't such moment of time <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, when the music doesn't play any longer. It is guaranteed that <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> &lt; <i>v</i><sub class="lower-index"><i>i</i> + 1</sub></span> <span class="tex-span">(<i>i</i> &lt; <i>m</i>)</span>.</p><p>The moment of time <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> means that Eugeny wants to know which song was playing during the <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th munite from the start of listening to the playlist.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers — the <span class="tex-span"><i>i</i></span>-th number must equal the number of the song that was playing during the <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th minute after Eugeny started listening to the play list.</p>





```input1
1 2
2 8
1 16

```




```input2
4 9
1 2
2 1
1 1
2 2
1 2 3 4 5 6 7 8 9

```




```output1
1
1

```




```output2
1
1
2
2
3
4
4
4
4

```


