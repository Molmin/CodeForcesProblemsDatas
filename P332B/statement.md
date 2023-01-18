## Description

<div><p>Reforms continue entering Berland. For example, during yesterday sitting the Berland Parliament approved as much as <span class="tex-span"><i>n</i></span> laws (each law has been assigned a unique number from 1 to <span class="tex-span"><i>n</i></span>). Today all these laws were put on the table of the President of Berland, G.W. Boosch, to be signed.</p><p>This time mr. Boosch plans to sign <span class="tex-span">2<i>k</i></span> laws. He decided to choose <span class="tex-font-style-bf">exactly two</span> non-intersecting segments of integers from 1 to <span class="tex-span"><i>n</i></span> of length <span class="tex-span"><i>k</i></span> and sign all laws, whose numbers fall into these segments. More formally, mr. Boosch is going to choose two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i> - <i>k</i> + 1, <i>b</i> - <i>a</i> ≥ <i>k</i>)</span> and sign all laws with numbers lying in the segments <span class="tex-span">[<i>a</i>;&nbsp;<i>a</i> + <i>k</i> - 1]</span> and <span class="tex-span">[<i>b</i>;&nbsp;<i>b</i> + <i>k</i> - 1]</span> (borders are included).</p><p>As mr. Boosch chooses the laws to sign, he of course considers the public opinion. Allberland Public Opinion Study Centre (APOSC) conducted opinion polls among the citizens, processed the results into a report and gave it to the president. The report contains the absurdity value for each law, in the public opinion. As mr. Boosch is a real patriot, he is keen on signing the laws with the maximum total absurdity. Help him.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 &lt; 2<i>k</i> ≤ <i>n</i></span>) — the number of laws accepted by the parliament and the length of one segment in the law list, correspondingly. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> — the absurdity of each law (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> — the beginning of segments that mr. Boosch should choose. That means that the president signs laws with numbers from segments <span class="tex-span">[<i>a</i>;&nbsp;<i>a</i> + <i>k</i> - 1]</span> and <span class="tex-span">[<i>b</i>;&nbsp;<i>b</i> + <i>k</i> - 1]</span>. If there are multiple solutions, print the one with the minimum number <span class="tex-span"><i>a</i></span>. If there still are multiple solutions, print the one with the minimum <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 &lt; 2<i>k</i> ≤ <i>n</i></span>) — the number of laws accepted by the parliament and the length of one segment in the law list, correspondingly. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span> — the absurdity of each law (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print two integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> — the beginning of segments that mr. Boosch should choose. That means that the president signs laws with numbers from segments <span class="tex-span">[<i>a</i>;&nbsp;<i>a</i> + <i>k</i> - 1]</span> and <span class="tex-span">[<i>b</i>;&nbsp;<i>b</i> + <i>k</i> - 1]</span>. If there are multiple solutions, print the one with the minimum number <span class="tex-span"><i>a</i></span>. If there still are multiple solutions, print the one with the minimum <span class="tex-span"><i>b</i></span>.</p>





```input1
5 2
3 6 1 1 6

```




```input2
6 2
1 1 1 1 1 1

```




```output1
1 4

```




```output2
1 3

```



## Note

<p>In the first sample mr. Boosch signs laws with numbers from segments [1;2] and [4;5]. The total absurdity of the signed laws equals <span class="tex-span">3 + 6 + 1 + 6 = 16</span>.</p><p>In the second sample mr. Boosch signs laws with numbers from segments [1;2] and [3;4]. The total absurdity of the signed laws equals <span class="tex-span">1 + 1 + 1 + 1 = 4</span>.</p>
