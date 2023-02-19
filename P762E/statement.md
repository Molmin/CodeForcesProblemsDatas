## Description

<div><p>In the lattice points of the coordinate line there are <span class="tex-span"><i>n</i></span> radio stations, the <span class="tex-span"><i>i</i></span>-th of which is described by three integers:</p><ul> <li> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> — the coordinate of the <span class="tex-span"><i>i</i></span>-th station on the line, </li><li> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> — the broadcasting range of the <span class="tex-span"><i>i</i></span>-th station, </li><li> <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> — the broadcasting frequency of the <span class="tex-span"><i>i</i></span>-th station. </li></ul><p>We will say that two radio stations with numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> reach each other, if the broadcasting range of each of them is more or equal to the distance between them. In other words <span class="tex-span"><i>min</i>(<i>r</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>) ≥ |<i>x</i><sub class="lower-index"><i>i</i></sub> - <i>x</i><sub class="lower-index"><i>j</i></sub>|</span>.</p><p>Let's call a pair of radio stations <span class="tex-span">(<i>i</i>, <i>j</i>)</span> bad if <span class="tex-span"><i>i</i> &lt; <i>j</i></span>, stations <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> reach each other and they are close in frequency, that is, <span class="tex-span">|<i>f</i><sub class="lower-index"><i>i</i></sub> - <i>f</i><sub class="lower-index"><i>j</i></sub>| ≤ <i>k</i></span>.</p><p>Find the number of bad pairs of radio stations.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10</span>) — the number of radio stations and the maximum difference in the frequencies for the pair of stations that reach each other to be considered bad.</p><p>In the next <span class="tex-span"><i>n</i></span> lines follow the descriptions of radio stations. Each line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinate of the <span class="tex-span"><i>i</i></span>-th radio station, it's broadcasting range and it's broadcasting frequency. <span class="tex-font-style-bf">No two radio stations will share a coordinate</span>.</p></div><div class="output-specification"><p>Output the number of bad pairs of radio stations.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ 10</span>) — the number of radio stations and the maximum difference in the frequencies for the pair of stations that reach each other to be considered bad.</p><p>In the next <span class="tex-span"><i>n</i></span> lines follow the descriptions of radio stations. Each line contains three integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — the coordinate of the <span class="tex-span"><i>i</i></span>-th radio station, it's broadcasting range and it's broadcasting frequency. <span class="tex-font-style-bf">No two radio stations will share a coordinate</span>.</p>

## Output

<p>Output the number of bad pairs of radio stations.</p>





```input1
3 2
1 3 10
3 2 5
4 10 8

```




```input2
3 3
1 3 10
3 2 5
4 10 8

```




```input3
5 1
1 3 2
2 2 4
3 2 1
4 2 1
5 3 3

```




```input4
5 1
1 5 2
2 5 4
3 5 1
4 5 1
5 5 3

```




```output1
1

```




```output2
2

```




```output3
2

```




```output4
5

```


