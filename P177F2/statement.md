## Description

<div><p>The Smart Beaver from ABBYY was offered a job of a screenwriter for the ongoing TV series. In particular, he needs to automate the hard decision: which main characters will get married by the end of the series.</p><p>There are <span class="tex-span"><i>n</i></span> single men and <span class="tex-span"><i>n</i></span> single women among the main characters. An opinion poll showed that viewers like several couples, and a marriage of any of them will make the audience happy. The Smart Beaver formalized this fact as <span class="tex-span"><i>k</i></span> triples of numbers <span class="tex-span">(<i>h</i>, <i>w</i>, <i>r</i>)</span>, where <span class="tex-span"><i>h</i></span> is the index of the man, <span class="tex-span"><i>w</i></span> is the index of the woman, and <span class="tex-span"><i>r</i></span> is the measure of the audience's delight in case of the marriage of this couple. The same poll showed that the marriage of any other couple will leave the audience indifferent, so the screenwriters decided not to include any such marriages in the plot.</p><p>The script allows you to arrange several marriages between the heroes or not to arrange marriages at all. A subset of some of the <span class="tex-span"><i>k</i></span> marriages is considered acceptable if each man and each woman is involved in at most one marriage of the subset (the series won't allow any divorces). The value of the acceptable set of marriages is the total delight the spectators will get from the marriages included in this set.</p><p>Obviously, there is a finite number of acceptable sets, and they all describe some variants of the script. The screenwriters do not want to choose a set with maximum value — it would make the plot too predictable. So the Smart Beaver offers the following option: sort all the acceptable sets in increasing order of value and choose the <span class="tex-span"><i>t</i></span>-th set from the sorted list. Thus, <span class="tex-span"><i>t</i> = 1</span> corresponds to a plot without marriages, <span class="tex-span"><i>t</i> = 2</span> — to a single marriage resulting in minimal delight for the audience, and so on.</p><p>Help the Beaver to implement the algorithm for selecting the desired set.</p></div><div class="input-specification"><p>The first input line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(100, <i>n</i><sup class="upper-index">2</sup>)</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 2·10<sup class="upper-index">5</sup></span>), separated by single spaces. Next <span class="tex-span"><i>k</i></span> lines contain triples of integers <span class="tex-span">(<i>h</i>, <i>w</i>, <i>r</i>)</span> <span class="tex-span">(1 ≤ <i>h</i>, <i>w</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>r</i> ≤ 1000)</span>, separated by single spaces, which describe the possible marriages. It is guaranteed that the input data is correct: <span class="tex-span"><i>t</i></span> doesn't exceed the total number of acceptable sets, and each pair <span class="tex-span">(<i>h</i>, <i>w</i>)</span> is present in at most one triple.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5</span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 20</span> </li></ul> </div><div class="output-specification"><p>Print a single number — the value of the <span class="tex-span"><i>t</i></span>-th acceptable variant.</p></div>

## Input

<p>The first input line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>min</i>(100, <i>n</i><sup class="upper-index">2</sup>)</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 2·10<sup class="upper-index">5</sup></span>), separated by single spaces. Next <span class="tex-span"><i>k</i></span> lines contain triples of integers <span class="tex-span">(<i>h</i>, <i>w</i>, <i>r</i>)</span> <span class="tex-span">(1 ≤ <i>h</i>, <i>w</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>r</i> ≤ 1000)</span>, separated by single spaces, which describe the possible marriages. It is guaranteed that the input data is correct: <span class="tex-span"><i>t</i></span> doesn't exceed the total number of acceptable sets, and each pair <span class="tex-span">(<i>h</i>, <i>w</i>)</span> is present in at most one triple.</p><p>The input limitations for getting 30 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5</span> </li></ul> <p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 20</span> </li></ul>

## Output

<p>Print a single number — the value of the <span class="tex-span"><i>t</i></span>-th acceptable variant.</p>





```input1
2 4 3
1 1 1
1 2 2
2 1 3
2 2 7

```




```input2
2 4 7
1 1 1
1 2 2
2 1 3
2 2 7

```




```output1
2

```




```output2
8

```



## Note

<p>The figure shows 7 acceptable sets of marriages that exist in the first sample. </p><center> <img class="tex-graphics" src="file://Rn9w6VZe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
