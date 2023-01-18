## Description

<div><p>The crowdedness of the discotheque would never stop our friends from having fun, but a bit more spaciousness won't hurt, will it?</p><p>The discotheque can be seen as an infinite <span class="tex-span"><i>xy</i></span>-plane, in which there are a total of <span class="tex-span"><i>n</i></span> dancers. Once someone starts moving around, they will move only inside their own movement range, which is a circular area <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span> described by a center <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> and a radius <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-font-style-bf">No two ranges' borders have more than one common point</span>, that is for every pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>) either ranges <span class="tex-span"><i>C</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>C</i><sub class="lower-index"><i>j</i></sub></span> are disjoint, or one of them is a subset of the other. Note that it's possible that two ranges' borders share a single common point, but no two dancers have exactly the same ranges.</p><p>Tsukihi, being one of them, defines the <span class="tex-font-style-underline">spaciousness</span> to be <span class="tex-font-style-bf">the area covered by an odd number of movement ranges of dancers who are moving</span>. An example is shown below, with shaded regions representing the <span class="tex-font-style-underline">spaciousness</span> if everyone moves at the same time.</p><center> <img class="tex-graphics" src="file://07LT7vXf.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>But no one keeps moving for the whole night after all, so the whole night's time is divided into two halves — before midnight and after midnight. Every dancer moves around in one half, while sitting down with friends in the other. The <span class="tex-font-style-underline">spaciousness</span> of two halves are calculated separately and their sum should, of course, be as large as possible. The following figure shows an optimal solution to the example above.</p><center> <img class="tex-graphics" src="file://1L31iYUn.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>By different plans of who dances in the first half and who does in the other, different sums of <span class="tex-font-style-underline">spaciousness</span> over two halves are achieved. You are to find the largest achievable value of this sum.</p></div><div class="input-specification"><p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the number of dancers.</p><p>The following <span class="tex-span"><i>n</i></span> lines each describes a dancer: the <span class="tex-span"><i>i</i></span>-th line among them contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), describing a circular movement range centered at <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> with radius <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>Output one decimal number — the largest achievable sum of <span class="tex-font-style-underline">spaciousness</span> over two halves of the night.</p><p>The output is considered correct if it has a relative or absolute error of at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://NFSOh737.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the number of dancers.</p><p>The following <span class="tex-span"><i>n</i></span> lines each describes a dancer: the <span class="tex-span"><i>i</i></span>-th line among them contains three space-separated integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">6</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>), describing a circular movement range centered at <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> with radius <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p>

## Output

<p>Output one decimal number — the largest achievable sum of <span class="tex-font-style-underline">spaciousness</span> over two halves of the night.</p><p>The output is considered correct if it has a relative or absolute error of at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>. Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://NFSOh737.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
5
2 1 6
0 4 1
2 -1 3
1 -2 1
4 -1 1

```




```input2
8
0 0 1
0 0 2
0 0 3
0 0 4
0 0 5
0 0 6
0 0 7
0 0 8

```




```output1
138.23007676

```




```output2
289.02652413

```



## Note

<p>The first sample corresponds to the illustrations in the legend.</p>
