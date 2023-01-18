## Description

<div><p><span class="tex-font-style-it">Please note that the memory limit differs from the standard.</span></p><p>You really love to listen to music. During the each of next <span class="tex-span"><i>s</i></span> days you will listen to exactly <span class="tex-span"><i>m</i></span> songs from the playlist that consists of exactly <span class="tex-span"><i>n</i></span> songs. Let's number the songs from the playlist with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. The quality of song number <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>On the <span class="tex-span"><i>i</i></span>-th day you choose some integer <span class="tex-span"><i>v</i></span> (<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>v</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>) and listen to songs number <span class="tex-span"><i>v</i>, <i>v</i> + 1, ..., <i>v</i> + <i>m</i> - 1</span>. On the <span class="tex-span"><i>i</i></span>-th day listening to one song with quality less than <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> increases your displeasure by exactly one.</p><p>Determine what minimum displeasure you can get on each of the <span class="tex-span"><i>s</i></span> next days. </p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) — the description of songs from the playlist. </p><p>The next line contains a single number <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of days that you consider.</p><p>The next <span class="tex-span"><i>s</i></span> lines contain three integers each <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>m</i> + 1</span>; <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) — the description of the parameters for the <span class="tex-span"><i>i</i></span>-th day. In order to calculate value <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>, you need to use formula: <img align="middle" class="tex-formula" src="file://VrF1nBDV.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> is the answer to the problem for day <span class="tex-span"><i>i</i></span>. Assume that <span class="tex-span"><i>ans</i><sub class="lower-index">0</sub> = 0</span>. </p></div><div class="output-specification"><p>Print exactly <span class="tex-span"><i>s</i></span> integers <span class="tex-span"><i>ans</i><sub class="lower-index">1</sub>, <i>ans</i><sub class="lower-index">2</sub>, ..., <i>ans</i><sub class="lower-index"><i>s</i></sub></span>, where <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> is the minimum displeasure that you can get on day <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) — the description of songs from the playlist. </p><p>The next line contains a single number <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>s</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of days that you consider.</p><p>The next <span class="tex-span"><i>s</i></span> lines contain three integers each <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>m</i> + 1</span>; <span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; 2<sup class="upper-index">30</sup></span>) — the description of the parameters for the <span class="tex-span"><i>i</i></span>-th day. In order to calculate value <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>, you need to use formula: <img align="middle" class="tex-formula" src="file://VrF1nBDV.png" style="max-width: 100.0%;max-height: 100.0%;">, where <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> is the answer to the problem for day <span class="tex-span"><i>i</i></span>. Assume that <span class="tex-span"><i>ans</i><sub class="lower-index">0</sub> = 0</span>. </p>

## Output

<p>Print exactly <span class="tex-span"><i>s</i></span> integers <span class="tex-span"><i>ans</i><sub class="lower-index">1</sub>, <i>ans</i><sub class="lower-index">2</sub>, ..., <i>ans</i><sub class="lower-index"><i>s</i></sub></span>, where <span class="tex-span"><i>ans</i><sub class="lower-index"><i>i</i></sub></span> is the minimum displeasure that you can get on day <span class="tex-span"><i>i</i></span>.</p>





```input1
5 3
1 2 1 2 3
5
1 1 2
1 3 2
1 3 3
1 3 5
1 3 1

```




```output1
2
0
2
3
1

```


